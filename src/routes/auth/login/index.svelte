<script lang="ts">
	import { onMount } from 'svelte';
	// import axios from 'axios'

	// import { PublicApi, Configuration } from '@ory/kratos-client';
	// const kratos = new PublicApi(new Configuration({ basePath: 'http://185.103.199.195:4433/' }));
	// http://185.103.199.195:4433/self-service/login/browser

	onMount(async () => {
		const urlParams = new URLSearchParams(location.search);

		const flowId = urlParams.get('flow');

		console.log('f', flowId);

		const getCsrf = await fetch(
			`http://185.103.199.195:4433/self-service/login/flows?id=${flowId}`,
			{
				// mode: 'no-cors',
				// headers: {
				//   'Access-Control-Allow-Origin': 'http://localhost:3100'
				// }
			}
		);
		const csrfRes = await getCsrf.json();

		const csrf = csrfRes.methods.password.config.fields.find((e) => e.name === 'csrf_token').value;

		console.log(csrf);
	});

	// let csrf: string = ''
</script>

<div class="login">
	<h1 class="login-title">Login.</h1>
	<form class="login-form">
		<input type="text" placeholder="Email" />
		<input type="password" placeholder="Password" />
		<button>Proceed to login</button>
	</form>
	<a href="http://185.103.199.195:4433/self-service/registration/browser">Go to registration</a>
</div>

<style lang="postcss">
	.login {
		@apply p-6 rounded-2xl bg-white w-80;
	}

	.login-title {
		@apply text-3xl text-gray-800 mb-12;
	}

	.login-form {
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
