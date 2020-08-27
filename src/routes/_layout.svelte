<script>
  import Nav from "../components/Nav.svelte";

  export let segment;
</script>

<style>
  .container {
    max-width: 36rem;
    padding: 0 1rem;
    margin: 3rem auto 6rem;
  }
</style>

<main class="container">
  <Nav {segment} />
  <slot />
</main>
