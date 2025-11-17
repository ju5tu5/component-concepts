<script>
  import { FdndLogo, Nav, SearchForm } from '$lib/index.js'
</script>

<header>
  <FdndLogo>
  {#snippet subtitle()}
  Component Concepts
  {/snippet}
  </FdndLogo>

  <Nav />

  <SearchForm />
</header>


<style>
  header {
    display: grid;
    grid-template-columns: min-content min-content auto;
    gap:1rem;
    container-type: inline-size;
  }
</style>