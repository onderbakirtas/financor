<script lang="ts">
	import Hero from '$lib/Hero.svelte';
	import Features from '$lib/Features.svelte';
	import Advantages from '$lib/Advantages.svelte';
</script>

<main>
	<Hero />
	<Features />
	<Advantages />
</main>

<style style lang="postcss">
	main {
		@apply mx-auto;
	}
</style>
