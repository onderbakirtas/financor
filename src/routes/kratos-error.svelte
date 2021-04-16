<script context="module">
	async function load({ page }) {
		console.log(page);
		return { page };
	}
</script>

<script>
	export let page;
</script>

<h1>{page}</h1>
