<script>

let {listItems} = $props()

</script>

<ul>
  {#each listItems as item }
    <li>{item}</li>
  {/each}
</ul>

<style>

</style>