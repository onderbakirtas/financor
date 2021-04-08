<nav class="menu">
	<a class="menu-item" href="#how">How It Works</a>
	<a class="menu-item" href="#advantages">Advantages</a>
	<a class="menu-item" href="#getit">Get It</a>
</nav>

<style lang="postcss">
	.menu {
		@apply hidden md:flex flex-col md:flex-row justify-around items-center;
		@apply h-screen w-full md:w-auto md:h-12;
	}

	.menu-item {
		@apply md:mx-2 px-2 py-0;
		@apply inline-flex duration-150;
		@apply text-gray-800 md:text-purple-200;
	}

	.menu-item:hover {
		@apply text-gray-500 md:text-white;
	}
</style>
