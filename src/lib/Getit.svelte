<script>
	import Apple from './Icons/Apple.svelte';
	import Dollar from './Icons/Dollar.svelte';
	import PlayStore from './Icons/PlayStore.svelte';
	import Windows from './Icons/Windows.svelte';
</script>

<div class="getit-container" id="getit">
	<section class="getit">
		<main class="getit-body">
			<h3 class="getit-title">Get The Best of <span>Your Money</span></h3>
			<article class="getit-content">
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate provident nulla
				similique, voluptates id harum deserunt corrupti ea officia sed totam ullam ex dicta
				tempora? Quas maiores consectetur obcaecati nam. Cupiditate provident nulla similique,
				voluptates id harum deserunt corrupti ea officia sed totam ullam ex dicta tempora? Quas
				maiores consectetur obcaecati nam.
			</article>
			<div class="getit-buttons">
				<button class="button">Launch Financor</button>
			</div>
		</main>
		<aside class="getit-phones">
			<img class="phone" src="../img/download-right2.png" alt="download" />
		</aside>
	</section>
</div>

<style lang="postcss">
	.getit {
		@apply rounded-3xl max-w-screen-lg mx-auto flex;
	}

	.getit-container {
		@apply w-full bg-purple-100 relative z-10;
	}

	.getit-body {
		@apply flex flex-col justify-start items-start flex-shrink-0;
		@apply px-8 md:px-12 py-14 md:py-20;
		@apply w-full md:w-3/5;
	}

	.getit-title {
		@apply font-bold text-purple-800;
		@apply text-3xl md:text-4xl;
		font-family: 'Jost', sans-serif;
	}

	.getit-content {
		@apply text-base md:text-lg;
		@apply mt-3 text-gray-600 leading-relaxed;
	}

	.getit-buttons {
		@apply mt-4 inline-flex items-start;
	}

	.button {
		@apply h-12 px-6 inline-flex items-center bg-gray-900 text-white rounded-lg duration-150;
		font-family: 'Jost', sans-serif;
	}

	.button:hover {
		@apply bg-gray-700;
	}

	.getit-phones {
		@apply items-end justify-end w-full;
		@apply hidden md:flex;
	}

	.getit-phones .phone {
		@apply h-96;
	}
</style>
