<section class="hero-container">
	<div class="hero-content">
		<article class="hero-text">
			<h1 class="hero-title">Secure your wallet, track what you spend.</h1>
			<p class="hero-p">
				With its intelligent organization capabilities, Financor helps you to save your precious $$$
				to spend it later for your beloved kittens.
			</p>
      <div class="hero-buttons">
        <button class="button apple">Apple</button>
        <button class="button android">Android</button>
        <button class="button windows">Windows</button>
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
    min-height: 800px;
		background: linear-gradient(150deg, #281483 15%, #8f6ed5 70%, #d782d9 94%);
	}

	.hero-shape {
		@apply -bottom-2 left-0 absolute right-0 z-10;
	}

	.hero-content {
		@apply container mx-auto max-w-screen-xl relative z-20 pt-8;
		@apply flex flex-col md:flex-row items-center;
	}

	.hero-text {
		@apply text-white w-8/12;
	}

	.hero-title {
		@apply font-bold leading-tight;
		font-family: 'Playfair Display', serif;
    font-size: 2.5rem;
	}

	.hero-p {
		@apply pt-6 text-xl;
	}

	.hero-phone {
    @apply mx-auto relative mt-8;
	}
  
  .hero-phone-shape {
    @apply block w-auto max-w-full h-auto relative z-20 pointer-events-none select-none;

  }
  
  .hero-phone-image {
    @apply absolute block top-0 left-3 rounded-3xl pointer-events-none select-none;
    height: 98%;
    top: 5px;
  }

  .hero-buttons {
    @apply mt-8 flex;
  }

  .button {
    @apply inline-flex px-6 py-2 bg-white mr-4 duration-200 text-purple-600;
    @apply rounded-lg;
  }

  .button:hover {
    @apply bg-opacity-90;
  }

</style>
