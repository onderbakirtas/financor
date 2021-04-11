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
		@apply px-4 pt-20 md:pt-40 pb-10 md:pb-32;
		--ggs: 2;
	}

	.advantages-container {
		@apply relative z-10 w-full bg-white;
	}

	.advantages-header {
		@apply text-center max-w-screen-md mx-auto;
	}

	.advantages-header h2 {
		@apply text-gray-800;
		@apply text-3xl md:text-4xl;
		font-family: 'Playfair Display', serif;
	}

	.advantages-header h2 > span {
		@apply text-purple-700;
	}

	.advantages-header p {
		@apply mt-4 md:mt-6;
		@apply text-lg md:text-xl md:leading-8;
		@apply text-gray-500;
	}

	.advantages-main {
		@apply flex mt-20;
		@apply flex-col md:flex-row;
	}

	.advantages-image {
		@apply w-full md:w-3/6;
		@apply flex justify-center;
	}

	.advantages-list {
		@apply pl-16;
	}

	.advantage {
		@apply flex mb-8 items-start;
	}

	.advantage-icon {
		@apply flex items-center justify-center flex-grow-0 flex-shrink-0;
		@apply w-28 h-28 rounded-full bg-purple-100;
		@apply text-purple-700;
	}

	.advantage-body {
		@apply flex flex-col ml-4 py-2;
	}

	.advantage-title {
		@apply text-xl font-semibold text-gray-800;
		font-family: 'Jost', sans-serif;
	}

	.advantage-text {
		@apply text-gray-600 text-lg mt-1;
	}
</style>
