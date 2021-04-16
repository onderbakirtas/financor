<script lang="ts">
	import { onMount } from 'svelte';

	let flowId = '';
	let csrf = '';
	let errors = [];

	let formObj;

	onMount(async () => {
		const urlParams = new URLSearchParams(location.search);

		flowId = urlParams.get('flow');

		console.log('f', flowId);

		const getCsrf = await fetch(
			`http://185.103.199.195:4433/self-service/registration/flows?id=${flowId}`,
			{
				// mode: 'no-cors',
				// headers: {
				//   'Access-Control-Allow-Origin': 'http://localhost:3100'
				// }
			}
		);
		const csrfRes = await getCsrf.json();

		console.log('csrf res:', csrfRes);

		// errors.push(...csrfRes.methods.password.config.messages);

		// console.log(errors);

		csrf = csrfRes.methods.password.config.fields.find((e) => e.name === 'csrf_token').value;

		console.log(csrf);
	});

	// const getFlow = async () => {

	// }

	function getContentLength(formData) {
		const formDataEntries = [...formData.entries()];

		const contentLength = formDataEntries.reduce((acc, [key, value]) => {
			if (typeof value === 'string') return acc + value.length;
			if (typeof value === 'object') return acc + value.size;

			return acc;
		}, 0);

		return contentLength;
	}

	let email = '';
	let passw = '';

	const handleRegister = async (event) => {
		let formData = new FormData();
		console.log(email, passw, csrf);
		formData.append('traits.email', email);
		formData.append('password', passw);
		formData.append('csrf_token', csrf);
		console.log(formData);
		const sendFormData = await fetch(
			`http://185.103.199.195:4433/self-service/registration/methods/password?flow=${flowId}`,
			{
				method: 'post',
				credentials: 'include',
				headers: {
					'Content-Type': 'application/x-www-form-urlencoded'
					// 'Access-Control-Allow-Credentials': 'true'
				},
				body: formData
			}
		);

		console.log(sendFormData);

		const formDataRes = await sendFormData.text();
		console.log(formDataRes);
	};
</script>

<div class="signup">
	<h1 class="signup-title">Register.</h1>
	<!-- <form on:submit|preventDefault={handleRegister} class="signup-form"> -->
	<form
		class="signup-form"
		action={`http://185.103.199.195:4433/self-service/registration/methods/password?flow=${flowId}`}
		method="POST"
		enctype="application/x-www-form-urlencoded"
	>
		<input type="text" placeholder="Email" name="traits.email" bind:value={email} />
		<input type="password" placeholder="Password" name="password" bind:value={passw} />
		<input type="hidden" name="csrf_token" value={csrf} />
		<button type="submit">Finish registration</button>
	</form>
</div>

<style lang="postcss">
	.signup {
		@apply p-6 rounded-2xl bg-white w-80;
	}

	.signup-title {
		@apply text-3xl text-gray-800 mb-12;
	}

	.signup-form {
		@apply flex flex-col w-full;
	}

	input {
		@apply w-full border-0 bg-gray-200 rounded-md block p-3 mb-4 box-border outline-none;
	}

	button {
		@apply block border-0 bg-blue-700 text-white rounded-md text-center py-3 cursor-pointer;
	}

	input,
	button {
		@apply font-sans;
	}
</style>
