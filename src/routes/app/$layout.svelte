<script>
	import Sidebar from '$lib/App/Sidebar/Sidebar.svelte';
</script>

<main class="app">
	<Sidebar />
	<div class="content">
		<slot />
	</div>
</main>

<style lang="postcss">
	.app {
		@apply flex items-start w-full;
	}

  .content {
    @apply flex-grow w-full;
  }
</style>
