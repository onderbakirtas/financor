<script>
	import Apple from './Icons/Apple.svelte';
	import Dollar from './Icons/Dollar.svelte';
	import PlayStore from './Icons/PlayStore.svelte';
	import Windows from './Icons/Windows.svelte';
</script>

<div class="getit-container">
	<section class="getit">
		<main class="getit-body">
			<h3 class="getit-title">Download <span>Financor</span> App</h3>
			<article class="getit-content">
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate provident nulla
				similique, voluptates id harum deserunt corrupti ea officia sed totam ullam ex dicta
				tempora? Quas maiores consectetur obcaecati nam. Cupiditate provident nulla similique,
				voluptates id harum deserunt corrupti ea officia sed totam ullam ex dicta tempora? Quas
				maiores consectetur obcaecati nam.
			</article>
			<div class="getit-buttons">
				<button class="button">
					<Apple />
				</button>
				<button class="button">
					<PlayStore />
				</button>
				<button class="button">
					<Windows />
				</button>
			</div>
		</main>
		<aside class="getit-phones">
			<img class="phone" src="../img/download-right2.png" alt="download" />
		</aside>
	</section>
</div>

<style lang="postcss">
	.getit {
		@apply bg-purple-700 rounded-3xl max-w-screen-lg mx-auto mt-32 flex;
	}

  .getit-container {
    @apply w-full bg-purple-700;
  }

	.getit-body {
		@apply px-12 py-20 w-3/5 flex flex-col justify-start items-start flex-shrink-0;
	}

	.getit-title {
		@apply text-4xl font-bold text-white;
		font-family: 'Jost', sans-serif;
	}

	.getit-content {
		@apply mt-3 text-lg text-purple-200;
	}

	.getit-buttons {
		@apply mt-4 inline-flex items-start;
	}

	.button {
		@apply h-12 w-12 p-2 inline-flex text-purple-50 duration-150;
	}

	.button + .button {
		@apply ml-4;
	}

	.button:hover {
		@apply text-purple-300;
	}

	.getit-phones {
		@apply flex items-end justify-end w-full;
	}

	.getit-phones .phone {
		@apply h-96;
	}
</style>
