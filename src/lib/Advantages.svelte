<script>
	import Dollar from './Icons/Dollar.svelte';
	import FileDocument from './Icons/FileDocument.svelte';
	import Trophy from './Icons/Trophy.svelte';
</script>

<div class="advantages-container" id="advantages">
	<section class="advantages">
		<header class="advantages-header">
			<h2>Advantages of <span>Financor</span></h2>
			<p>
				You have full control on how you create accounts, categories and savings. The only thing you
				need to do is add expense/income, rest is done by Financor.
			</p>
		</header>
		<main class="advantages-main">
			<aside class="advantages-image">
				<img src="../img/about.png" alt="advantage" />
			</aside>
			<section class="advantages-list">
				<div class="advantage">
					<span class="advantage-icon">
						<Dollar />
					</span>
					<div class="advantage-body">
						<h3 class="advantage-title">Some Advantage Title</h3>
						<p class="advantage-text">
							Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub
							indxgo juice poutine.
						</p>
					</div>
				</div>
				<div class="advantage">
					<span class="advantage-icon">
						<FileDocument />
					</span>
					<div class="advantage-body">
						<h3 class="advantage-title">Some Advantage Title</h3>
						<p class="advantage-text">
							Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub
							indxgo juice poutine.
						</p>
					</div>
				</div>
				<div class="advantage">
					<span class="advantage-icon">
						<Trophy />
					</span>
					<div class="advantage-body">
						<h3 class="advantage-title">Some Advantage Title</h3>
						<p class="advantage-text">
							Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub
							indxgo juice poutine.
						</p>
					</div>
				</div>
			</section>
		</main>
	</section>
</div>

<style lang="postcss">
	.advantages {
		@apply container max-w-screen-xl mx-auto;
		@apply py-14 md:py-24 xl:py-32 px-4;
		--ggs: 1.5;
	}

	@media (max-width: 768) {
		.advantages {
			--ggs: 2;
		}
	}

	.advantages-container {
		@apply relative z-10 w-full bg-gray-50;
	}

	.advantages-header {
		@apply text-center max-w-screen-md mx-auto;
		@apply pb-12 md:pb-20;
	}

	.advantages-header h2 {
		@apply text-gray-800;
		@apply text-3xl md:text-4xl xl:text-5xl;
		font-family: 'Playfair Display', serif;
	}

	.advantages-header h2 > span {
		@apply text-purple-700;
	}

	.advantages-header p {
		@apply mt-4 md:mt-6;
		@apply text-base md:text-lg xl:text-xl;
		@apply text-gray-500;
	}

	.advantages-main {
		@apply flex;
		@apply flex-col lg:flex-row;
		@apply items-start lg:items-center;
	}

	.advantages-image {
		@apply w-full lg:w-3/6;
		@apply md:px-16 lg:px-0;
		@apply flex-shrink-0 flex-grow self-center;
	}

	.advantages-image > img {
		@apply w-full h-auto;
	}

	.advantages-list {
		@apply lg:pl-16 mt-14 lg:mt-0;
	}

	.advantage {
		@apply flex;
		@apply flex-col md:flex-row;
		@apply items-center md:items-start;
		@apply text-center md:text-left;
	}

	.advantage + .advantage {
		@apply mt-10;
	}

	.advantage-icon {
		@apply flex items-center justify-center flex-grow-0 flex-shrink-0;
		@apply w-24 xl:w-28 h-24 xl:h-28;
		@apply text-blue-50 bg-purple-600 rounded-full;
	}

	.advantage-body {
		@apply flex flex-col;
		@apply pt-2 md:pt-1 md:pb-1 md:ml-4;
	}

	.advantage-title {
		@apply text-lg md:text-xl font-semibold text-gray-800 leading-relaxed;
		font-family: 'Jost', sans-serif;
	}

	.advantage-text {
		@apply text-base xl:text-lg;
		@apply mt-1;
		@apply text-gray-500;
	}
</style>
