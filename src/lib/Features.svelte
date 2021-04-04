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

<style lang="postcss">
	.features {
		@apply container max-w-screen-xl mx-auto py-40;
	}

	.features-header {
		@apply text-center max-w-screen-md mx-auto;
	}

	.features-header h2 {
		@apply text-4xl text-gray-800;
		font-family: 'Playfair Display', serif;
	}

	.features-header h2 > span {
		@apply text-purple-700;
	}

	.features-header p {
		@apply mt-6 text-xl text-gray-500 leading-8;
	}

	.features-main {
		@apply flex max-w-screen-xl mt-20 items-center;
	}

	.feature {
		@apply flex flex-col mb-8;
	}

	.features-main .left .feature {
		@apply justify-end items-end text-right;
	}

	.features-main .right .feature {
		@apply justify-start items-start;
	}

	.features-main .left {
    @apply pr-8;
  }
  
	.features-main .right {
    @apply pl-8;
  }

	.features-main .left,
	.features-main .right {
		@apply w-2/6;
	}

	.features-main .center {
		@apply w-2/6 flex items-center justify-center relative;
	}

	.features-main .center::before {
		content: '';
		@apply block absolute z-0;
		@apply w-96 h-96 bg-purple-700 rounded-full;
	}

	.features-main .center img {
		@apply relative z-10;
	}

	.feature-icon {
		@apply inline-flex items-center justify-center;
		@apply rounded-3xl h-20 w-20;
		@apply bg-purple-200 text-purple-800;
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
