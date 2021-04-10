<script lang="ts">
	import Logo from './Logo.svelte';
	import NavbarCta from './NavbarCta.svelte';
	import NavbarMenu from './NavbarMenu.svelte';

	let y = 0;
  let showable = true;


</script>

<svelte:window bind:scrollY={y} />

<nav class="navbar" class:scrolled={y > 100}>
	<Logo inverted={y > 100} />
	<NavbarMenu />
	<NavbarCta />
</nav>

<style lang="postcss">
	.navbar {
		@apply px-3 md:px-6;
		@apply h-14 md:h-16;
		@apply flex justify-between items-center flex-wrap md:flex-nowrap;
		@apply fixed w-full z-40 duration-150;
		@apply border-b border-transparent;
		@apply bg-white bg-opacity-90 md:bg-transparent md:bg-opacity-100;
		font-family: 'Jost', sans-serif;
	}

	.navbar.scrolled {
		@apply bg-white bg-opacity-90 border-gray-200;
		backdrop-filter: blur(10px);
	}

	.navbar.scrolled :global(.logo-txt) {
		@apply text-gray-700;
	}

	.navbar.scrolled :global(.menu-item) {
		@apply text-gray-800;
	}

	.navbar.scrolled :global(.menu-item:hover) {
		@apply text-gray-500;
	}

	.navbar.scrolled :global(.navbar-cta) {
		@apply bg-purple-700 text-white;
	}
</style>
