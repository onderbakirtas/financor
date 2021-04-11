<script lang="ts">
	export let inverted = true;

	$: logoPath = inverted ? '../img/wallet-c.svg' : '../img/wallet-a.svg';
</script>

<a class="logo" href="/">
	<img class="logo-img" src={logoPath} alt="Logo" />
	<img class="logo-img-m" src="../img/wallet-c.svg" alt="Logo" />
	<span class="logo-txt">Financor</span>
</a>

<style lang="postcss">
	.logo {
		@apply inline-flex items-center justify-center md:justify-start ;
	}

	.logo-img {
		@apply h-10 hidden md:inline-block ;
	}

	.logo-img-m {
		@apply h-9 inline-block md:hidden;
	}

	.logo-txt {
		@apply text-gray-700 md:text-white;
		@apply ml-1 md:ml-2 font-bold;
		@apply text-xl md:text-2xl;
		font-family: 'Jost', sans-serif;
		font-weight: 700;
	}
</style>
