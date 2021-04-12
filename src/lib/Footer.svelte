<footer class="footer-container">
	<div class="footer">
		<div class="footer-subscribe">
			<h6 class="subscribe-title">Poking Service</h6>
			<div class="subscribe-body">
				<input type="text" placeholder="Your precious email address..." />
				<button>Get Notified</button>
			</div>
			<p class="subscribe-footer">You will only be notified, not spammed.</p>
		</div>
		<div class="footer-social">
			<button>
				<img src="../img/facebook.png" alt="facebook button" />
			</button>
			<button>
				<img src="../img/twitter.png" alt="twitter button" />
			</button>
			<button>
				<img src="../img/telegram.png" alt="telegram button" />
			</button>
		</div>
	</div>
</footer>
<div class="footer-bottomline">
	<div class="footer-meta">
		<span class="copy">&copy; 2021.</span>
		<a class="link" href="/">
			<img src="../img/wallet-a.svg" alt="logo" />
		</a>
		<span class="meta">Helps you to save.</span>
	</div>
</div>

<style lang="postcss">
	.footer-container {
		@apply bg-gray-900 relative z-10;
	}

	.footer {
		@apply max-w-screen-xl mx-auto flex justify-between items-center;
		@apply flex-col md:flex-row;
		@apply py-8 px-4 md:py-12;
	}

	.footer-subscribe {
		@apply w-full;
		@apply text-center md:text-left;
	}

	.subscribe-title {
		@apply text-white font-bold mb-2;
		@apply text-base md:text-lg;
	}

	.subscribe-body {
		@apply flex justify-start;
		@apply items-stretch md:items-center;
		@apply flex-col md:flex-row;
	}

	.subscribe-body input {
		@apply bg-gray-50 h-12 outline-none p-4 rounded-lg duration-150 inline-block w-72 appearance-none;
		@apply border-4 border-solid border-gray-50;
		@apply w-full md:w-72;
	}
	.subscribe-body input:focus {
		@apply bg-white border-pink-400;
	}

	.subscribe-body button {
		@apply bg-pink-700 text-pink-50 h-12 rounded-lg px-6 duration-150;
		@apply mt-3 md:mt-0 md:ml-2;
		font-family: 'Jost', sans-serif;
	}

	.subscribe-body button:hover {
		@apply bg-pink-500;
	}

	.subscribe-footer {
		@apply mt-2 text-gray-400;
	}

	.footer-social {
		@apply flex;
		@apply mt-6 md:mt-0;
		@apply py-2 md:py-0;
	}

	.footer-social button {
		@apply w-12 h-12 p-4;
		@apply inline-flex justify-center items-end;
		@apply bg-gray-800 rounded-full duration-150;
	}

	.footer-social button > img {
		@apply opacity-80 duration-150;
	}

	.footer-social button + button {
		@apply ml-3;
	}

	.footer-social button:hover {
		@apply bg-gray-700;
	}

	.footer-social button:hover > img {
		@apply opacity-100;
	}

	.footer-bottomline {
		@apply bg-gray-800 h-16 flex items-center fixed bottom-0 left-0 right-0 w-full z-0;
		@apply px-4;
	}

	.footer-meta {
		@apply max-w-screen-xl container flex-row-reverse mx-auto flex items-center;
		@apply justify-start md:justify-between;
	}

	.link {
		@apply inline-flex items-center;
		@apply order-1 md:order-2;
		@apply ml-auto md:ml-0;
	}

	/* .link span {
		@apply inline-block text-2xl font-bold text-white;
		font-family: 'Jost', sans-serif;
	} */

	.link img {
		@apply inline-block h-10 opacity-90;
	}

	.meta {
		@apply order-3 md:order-3;
	}

	.copy {
		@apply text-right;
		@apply w-auto;
		@apply order-2 md:order-1;
		@apply ml-1 md:ml-0;
	}

	.meta,
	.copy {
		@apply text-gray-300 md:w-40;
	}
</style>
