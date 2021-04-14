<script>
	import { page } from '$app/stores';
	import Logo from '$lib/Logo/Logo.svelte';
</script>

<aside class="sidebar">
	<Logo />
	<a href="/app" class="cta">Add Transaction</a>
	<a class="action" href="/app/home" class:active={$page.path === '/app/home'}>Home</a>
	<a class="action" href="/app">Transactions</a>
	<a class="action" href="/app">Budgets</a>
	<a class="action" href="/app">Settings</a>
</aside>

<style lang="postcss">
	.sidebar {
		@apply w-72 border-r border-gray-300 h-screen flex flex-col py-3 px-6;
	}

	.sidebar :global(.logo) {
		@apply mb-6;
	}

	.sidebar :global(.logo-txt) {
		@apply text-gray-800;
	}

	.action {
		@apply inline-block py-2 px-4 rounded-md duration-100;
	}

	.action + .action {
		@apply mt-2;
	}

	.action:hover {
		@apply bg-gray-100 text-blue-700;
	}

  .action.active {
    @apply text-blue-700;
  }

	.cta {
		@apply block mb-5 rounded-md bg-blue-700 text-white py-3 text-center duration-100;
	}

	.cta:hover {
		@apply bg-blue-800;
	}
</style>
