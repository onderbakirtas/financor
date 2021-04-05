<script lang="ts">
	export let inverted = true;

	$: logoPath = inverted ? '../img/logo-p.png' : '../img/logo-w.png';
</script>

<a class="logo" href="/">
	<img class="logo-img" src={logoPath} alt="Logo" />
	<span class="logo-txt">Financor</span>
</a>

<style lang="postcss">
	.logo {
		@apply inline-flex text-2xl items-center;
	}

	.logo-img {
		@apply h-10 inline-block;
	}

	.logo-txt {
		@apply ml-2 font-bold text-white;
		font-family: 'Jost', sans-serif;
		font-weight: 700;
	}
</style>
