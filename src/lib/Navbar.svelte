<script>
import Logo from "./Logo.svelte";
import NavbarCta from "./NavbarCta.svelte";
import NavbarMenu from "./NavbarMenu.svelte";

</script>
<nav class="navbar">
  <Logo />
  <NavbarMenu />
  <NavbarCta />
</nav>

<style lang="postcss">
.navbar {
  @apply py-3 px-6 flex justify-between items-center fixed w-full z-50;
  font-family: 'Jost', sans-serif;
}
</style>