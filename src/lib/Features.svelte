<div class="features-container" id="how">
	<section class="features">
		<header class="features-header">
			<h2>How <span>Financor</span> Works</h2>
			<p>
				You have full control on how you create accounts, categories and savings. The only thing you
				need to do is add expense/income, rest is done with Financor's intelligent organiziting
				capabilities.
			</p>
		</header>
		<main class="features-main">
			<div class="left">
				<div class="feature">
					<span class="feature-icon">1</span>
					<h3 class="feature-title">Add Your Expense</h3>
					<p class="feature-text">Easily add your expense/income with one tap.</p>
				</div>
				<div class="feature">
					<span class="feature-icon">2</span>
					<h3 class="feature-title">Add Your Expense</h3>
					<p class="feature-text">Easily add your expense/income with one tap.</p>
				</div>
			</div>
			<div class="center">
				<img src="../img/feature-image.png" alt="feature" />
			</div>
			<div class="right">
				<div class="feature">
					<span class="feature-icon">3</span>
					<h3 class="feature-title">Add Your Expense</h3>
					<p class="feature-text">Easily add your expense/income with one tap.</p>
				</div>
				<div class="feature">
					<span class="feature-icon">4</span>
					<h3 class="feature-title">Add Your Expense</h3>
					<p class="feature-text">Easily add your expense/income with one tap.</p>
				</div>
			</div>
		</main>
	</section>
</div>

<style lang="postcss">
	.features {
		@apply container max-w-screen-xl mx-auto;
		@apply pt-16 md:pt-40 px-4;
	}

	.features-container {
		@apply relative z-10 bg-white;
	}

	.features-header {
		@apply text-center max-w-screen-md mx-auto;
	}

	.features-header h2 {
		@apply text-gray-800;
		@apply text-3xl md:text-4xl;
		font-family: 'Playfair Display', serif;
	}

	.features-header h2 > span {
		@apply text-purple-700;
	}

	.features-header p {
		@apply mt-4 md:mt-6;
		@apply text-lg md:text-xl md:leading-8;
		@apply text-gray-500;
	}

	.features-main {
		@apply flex max-w-screen-xl mt-20 items-center;
		@apply flex-col md:flex-row;
	}

	.features-main .left .feature {
		@apply justify-end items-end text-right;
	}

	.features-main .left {
		@apply pr-8;
		@apply order-2 md:order-1;
	}

	.features-main .center {
		@apply w-2/6 flex items-center justify-center relative;
		@apply order-1 md:order-2;
	}

	.features-main .right {
		@apply pl-8;
		@apply order-3 md:order-3;
	}

	.features-main .left,
	.features-main .right {
		@apply w-2/6;
	}

	.features-main .center::before {
		content: '';
		@apply block absolute z-0;
		@apply w-96 h-96 bg-purple-700 rounded-full;
	}

	.features-main .center img {
		@apply relative z-10;
	}
	.feature {
		@apply flex flex-col mb-8;
	}

	.features-main .right .feature {
		@apply justify-start items-start;
	}

	.feature-icon {
		@apply inline-flex items-center justify-center;
		@apply rounded-2xl h-20 w-20;
		@apply bg-purple-100 text-purple-700;
		@apply text-4xl font-bold;
	}

	.feature-title {
		@apply text-xl font-bold text-gray-800;
		@apply mt-4;
		font-family: 'Jost', sans-serif;
	}

	.feature-text {
		@apply mt-1 text-gray-600 text-lg;
	}
</style>
