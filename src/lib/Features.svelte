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
		@apply py-14 md:py-24 xl:py-32 px-4;
	}

	.features-container {
		@apply relative z-10 bg-white;
	}

	.features-header {
		@apply text-center max-w-screen-md mx-auto;
	}

	.features-header h2 {
		@apply text-gray-800;
		@apply text-3xl md:text-4xl xl:text-5xl;
		font-family: 'Playfair Display', serif;
	}

	.features-header h2 > span {
		@apply text-purple-700;
	}

	.features-header p {
		@apply mt-5 text-gray-500 leading-relaxed;
		@apply text-base md:text-lg xl:text-xl;
	}

	.features-main {
		@apply flex items-center max-w-screen-xl;
		@apply flex-col md:flex-row;
		@apply mt-14 md:mt-20;
	}

	.features-main .left {
		@apply md:pr-8;
		@apply mb-6 md:mb-0;
		@apply order-2 md:order-1;
	}

	.features-main .center {
		@apply flex items-center justify-center relative;
		@apply w-full md:w-2/6;
		@apply order-1 md:order-2;
		@apply mb-14 md:mb-0;
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
		@apply mb-6 xl:mb-8;
	}

	.feature + .feature {
		@apply mb-0;
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
		@apply h-16 xl:h-20 w-16 xl:w-20;
		@apply text-2xl xl:text-4xl;
	}

	.feature-body {
		@apply ml-4 md:m-0;
	}

	.feature-title {
		@apply text-lg xl:text-xl;
		@apply md:mt-2 xl:mt-4;
		@apply font-bold text-gray-800 leading-relaxed;
		font-family: 'Jost', sans-serif;
	}

	.feature-text {
		@apply text-base xl:text-lg;
		@apply md:mt-1;
		@apply text-gray-600 leading-snug;
	}
</style>
