<section class="hero-container">
	<div class="hero-content">
		<article class="hero-text">
			<h1 class="hero-title">Secure your wallet, track what you spend.</h1>
			<p class="hero-p">
				With its intelligent organization capabilities, Financor helps you to save your precious $$$
				to spend it later for your beloved kittens.
			</p>
			<div class="hero-buttons">
				<button class="button apple">Launch Financor</button>
				<button class="button button-outlined">Explore for more</button>
			</div>
		</article>
		<aside class="hero-phone">
			<img class="hero-phone-shape" src="../img/iphone-x-frame.png" alt="" />
			<img class="hero-phone-image" src="../img/top-screen-6.png" alt="some" />
		</aside>
	</div>
	<div class="hero-shape">
		<img src="../img/waves-shape.svg" alt="shape" />
	</div>
</section>

<style lang="postcss">
	.hero-container {
		@apply relative bg-cover bg-top z-10 h-auto;
		@apply pt-14 md:pt-16;
		@apply pb-12 md:pb-36;
		background: linear-gradient(150deg, #281483 15%, #8f6ed5 70%, #d782d9 94%);
	}

	.hero-shape {
		@apply bottom-0 left-0 absolute right-0 z-10;
	}

	.hero-content {
		@apply container mx-auto max-w-screen-xl relative z-20;
		@apply flex items-center;
		@apply flex-col md:flex-row;
		@apply pt-12 md:pt-8;
		@apply pb-16 md:pb-0;
		@apply px-4 md:px-6;
	}

	.hero-text {
		@apply text-white;
		@apply w-full md:w-10/12;
		@apply pr-0 md:pr-8 xl:pr-0;
	}

	.hero-title {
		@apply text-3xl lg:text-4xl;
		@apply font-bold leading-tight;
		font-family: 'Playfair Display', serif;
	}

	.hero-p {
		@apply text-indigo-200;
		@apply pt-4 md:pt-6;
		@apply text-lg xl:text-xl;
	}

	.hero-phone {
		@apply relative;
		@apply mx-20 md:mx-auto;
		@apply mt-20 md:mt-8;
	}

	.hero-phone-shape {
		@apply block w-auto max-w-full h-auto relative z-20 pointer-events-none select-none;
	}

	.hero-phone-image {
		@apply absolute block left-4 rounded-3xl pointer-events-none select-none;
		height: 95%;
		top: 12px;
	}

	.hero-buttons {
		@apply mt-8 flex;
	}

	.button {
		font-family: 'Jost', sans-serif;
		box-shadow: none;
		@apply inline-flex items-center;
		@apply rounded-md bg-white text-gray-700 duration-200 leading-none;
		@apply md:text-lg;
		@apply px-5 md:px-6;
		@apply h-11 md:h-12 xl:h-14;
	}
	.button:hover {
		@apply bg-indigo-100;
	}

	.button-outlined {
		@apply bg-transparent border-2 border-indigo-100 text-indigo-200 ml-4;
	}

	.button-outlined:hover {
		@apply bg-white bg-opacity-20 text-white;
		box-shadow: none;
	}
</style>
