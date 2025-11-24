<script>
  import { List, TodoForm } from '$lib'
  let {listItems = $bindable([])} = $props()
</script>


<List bind:listItems />
<TodoForm bind:listItems />

<style>

</style>