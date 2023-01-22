<script lang="ts">
	let count = 0;

	const increment = (): void => {
		count += 1;
	};
</script>

<button on:click={increment}>
	Clicks: {count}
</button>

<style style lang="postcss">
	button {
		font-size: inherit;
		@apply py-0 px-2 mx-0 my-0;
		@apply font-serif text-xl;
		@apply py-4 px-8 text-green-500 bg-purple-500 bg-opacity-10;
		@apply rounded-full;
		@apply border-opacity-100;
		@apply outline-none;
		@apply w-48;
		height: 60px;
		font-variant-numeric: tabular-nums;
	}

	button:hover {
		@apply bg-yellow-400;
	}

	button:active {
		@apply bg-red-500 bg-opacity-20;
	}
</style>
