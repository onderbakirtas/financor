<script lang="ts">
	import logoWhite from './images/wallet-a.svg';
	import logoColor from './images/wallet-c.svg';

	export let inverted = true;

	$: logoPath = inverted ? logoColor : logoWhite;
</script>

<a class="logo" href="/">
	<img class="logo-img" src={logoPath} alt="Logo" />
	<img class="logo-img-m" src={logoColor} alt="Logo" />
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
		font-weight: 700;
	}
</style>
