<script lang="ts">
	import Navbar from '$lib/Navbar.svelte';
	import Hero from '$lib/Hero/Hero.svelte';
	import Features from '$lib/Features/Features.svelte';
	import Advantages from '$lib/Advantages/Advantages.svelte';
	import Getit from '$lib/Getit/Getit.svelte';
	import Footer from '$lib/Footer/Footer.svelte';

	import '../global.css';
</script>

<Navbar />
<main>
	<Hero />
	<Features />
	<Advantages />
	<Getit />
	<Footer />
</main>

<style style lang="postcss">
	main {
		@apply mx-auto pb-16;
	}
</style>
