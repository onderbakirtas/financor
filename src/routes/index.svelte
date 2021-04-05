<script lang="ts">
	import Hero from '$lib/Hero.svelte';
	import Features from '$lib/Features.svelte';
	import Advantages from '$lib/Advantages.svelte';
	import Getit from '$lib/Getit.svelte';
	import Footer from '$lib/Footer.svelte';
</script>

<main>
	<Hero />
	<Features />
	<Advantages />
	<Getit />
	<Footer />
</main>

<style style lang="postcss">
	main {
		@apply mx-auto;
	}
</style>
