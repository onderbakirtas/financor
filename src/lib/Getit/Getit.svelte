<script lang="ts">
	import handPhone from './images/download-right2.png';
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
			<img class="phone" src={handPhone} alt="download" />
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
		@apply px-6 lg:px-12 py-14 lg:py-20;
		@apply w-full lg:w-3/5;
	}

	.getit-title {
		@apply font-bold text-purple-800;
		@apply text-2xl md:text-3xl xl:text-4xl;
	}

	.getit-content {
		@apply text-base lg:text-lg;
		@apply mt-2 md:mt-3 text-gray-500 leading-relaxed;
	}

	.getit-buttons {
		@apply mt-6 inline-flex items-start;
	}

	.button {
		@apply inline-flex items-center bg-gray-900 text-white rounded-lg duration-150;
		@apply h-11 md:h-12 xl:h-14;
		@apply px-5 md:px-6 xl:px-8;
	}

	.button:hover {
		@apply bg-gray-700;
	}

	.getit-phones {
		@apply items-end justify-end w-full;
		@apply hidden lg:flex;
	}

	.getit-phones .phone {
		@apply h-96;
	}
</style>
