<script>
	import Facebook from './Icons/Facebook.svelte';
	import Telegram from './Icons/Telegram.svelte';
	import Twitter from './Icons/Twitter.svelte';
</script>

<footer class="footer">
	<div class="footer-container">
		<div class="footer-subscribe">
			<div class="subscribe-body">
				<input type="text" placeholder="Email address..." />
				<button>Get Notified</button>
			</div>
			<p class="subscribe-footer">We don't spam, only three or four mails for you.</p>
		</div>
		<div class="footer-social">
			<button>
				<Facebook />
			</button>
			<button>
				<Twitter />
			</button>
			<button>
				<Telegram />
			</button>
		</div>
	</div>
</footer>
<div class="footer-bottomline">
  <div class="footer-meta">
    <span class="copy">&copy; 2021.</span>
    <a class="link" href="/">
      <!-- <img src="../img/logo-w.png" alt="logo"> -->
      <span>Financor</span>
    </a>
    <span class="meta">Helps you to save.</span>
  </div>
</div>

<style lang="postcss">
	.footer {
		@apply bg-purple-900;
	}

	.footer-container {
		@apply max-w-screen-xl mx-auto flex justify-between items-center h-40;
	}

	.subscribe-body {
    @apply flex justify-start items-center;
	}

  .subscribe-body input {
    @apply bg-gray-50 h-12 outline-none p-4 rounded-lg duration-150 inline-block w-72;
    @apply border-4 border-solid border-gray-50;
  }
  .subscribe-body input:focus {
    @apply bg-white border-pink-400;
  }

  .subscribe-body button {
    @apply bg-pink-500 text-indigo-100 h-12 rounded-lg ml-2 px-6 font-bold duration-150;
  }

  .subscribe-body button:hover {
    @apply bg-pink-600;
  }

  .subscribe-footer {
    @apply mt-2 text-purple-300;
  }

	.footer-social button {
    @apply w-10 h-10 ml-3 p-3;
		@apply inline-flex justify-center items-end;
		@apply bg-purple-600 text-purple-100 rounded-full duration-150;
	}

	.footer-social button:hover {
		@apply bg-purple-500 text-white;
	}

  .footer-bottomline {
    @apply bg-gray-900 h-16 flex items-center;
  }

  .footer-meta {
    @apply max-w-screen-xl container flex-row-reverse mx-auto flex justify-between items-center;
  }

  .link {
    @apply inline-flex items-center;
  }

  .link span {
    @apply inline-block text-2xl font-bold text-white;
    font-family: 'Jost', sans-serif;
  }

  .meta, .copy {
    @apply text-gray-300 w-40;
  }

  .copy {
    @apply text-right
  }
</style>
