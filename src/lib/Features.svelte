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
					<main class="feature-body">
						<h3 class="feature-title">Add Your Expense</h3>
						<p class="feature-text">Easily add your expense/income with one tap.</p>
					</main>
				</div>
				<div class="feature">
					<span class="feature-icon">2</span>
					<main class="feature-body">
						<h3 class="feature-title">Add Your Expense</h3>
						<p class="feature-text">Easily add your expense/income with one tap.</p>
					</main>
				</div>
			</div>
			<div class="center">
				<img src="../img/feature-image.png" alt="feature" />
			</div>
			<div class="right">
				<div class="feature">
					<span class="feature-icon">3</span>
					<main class="feature-body">
						<h3 class="feature-title">Add Your Expense</h3>
						<p class="feature-text">Easily add your expense/income with one tap.</p>
					</main>
				</div>
				<div class="feature">
					<span class="feature-icon">4</span>
					<main class="feature-body">
						<h3 class="feature-title">Add Your Expense</h3>
						<p class="feature-text">Easily add your expense/income with one tap.</p>
					</main>
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

	.features-main .left {
		@apply md:pr-8;
		@apply order-2 md:order-1;
	}

	.features-main .center {
		@apply flex items-center justify-center relative;
		@apply w-full md:w-2/6;
		@apply order-1 md:order-2;
		@apply mb-8 md:mb-0;
	}

	.features-main .right {
		@apply md:pl-8;
		@apply order-3 md:order-3;
	}

	.features-main .left,
	.features-main .right {
		@apply w-full md:w-2/6;
	}

	.features-main .center::before,
	.features-main .center::after {
		content: '';
		@apply absolute rounded-full block;
	}

	.features-main .center::before {
		content: '';
		padding-top: 100%;
		@apply block absolute z-0;
		@apply bg-purple-100 rounded-full;
		@apply w-full;
	}

	.features-main .center::after {
		padding-top: 83.333333%;
		@apply z-20 bg-purple-700 w-10/12;
	}

	.features-main .center img {
		@apply relative z-30;
		@apply w-5/6 md:w-80;
	}
	.feature {
		@apply flex items-start;
		@apply flex-row md:flex-col;
		@apply mb-6 md:mb-8;
	}

	.features-main .right .feature {
		@apply justify-start items-start;
	}

	.features-main .left .feature {
		@apply items-start md:items-end;
		@apply justify-start md:justify-end;
		@apply text-left md:text-right;
	}

	.feature-icon {
		@apply bg-purple-100 text-purple-700 rounded-2xl font-bold;
		@apply inline-flex items-center justify-center flex-shrink-0 flex-grow-0;
		@apply h-16 md:h-20 w-16 md:w-20;
		@apply text-2xl md:text-4xl;
	}

	.feature-body {
		@apply ml-4 md:m-0;
	}

	.feature-title {
		@apply text-lg md:text-xl;
		@apply md:mt-4;
		@apply font-bold text-gray-800 leading-relaxed;
		font-family: 'Jost', sans-serif;
	}

	.feature-text {
		@apply text-base md:text-lg;
		@apply md:mt-1;
		@apply text-gray-600 leading-snug;
	}
</style>
