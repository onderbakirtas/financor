<script>
	import Facebook from './Icons/Facebook.svelte';
	import Telegram from './Icons/Telegram.svelte';
	import Twitter from './Icons/Twitter.svelte';
</script>

<footer class="footer">
	<div class="footer-container">
		<div class="footer-subscribe">
			<span class="subscribe-title">Get Notified</span>
			<div class="subscribe-body">
				<input type="text" />
				<button>Subscribe</button>
				<p>We don't spam, only three or four mails for you.</p>
			</div>
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

<style lang="postcss">
	.footer {
		@apply bg-purple-200 h-80;
	}
</style>
