<script>
  let { listItems = $bindable([]) } = $props()

  let todo = $state()

	function addToDo() {
		listItems.push(todo)
	}
</script>

<form action="/">
  <fieldset>
    <legend class="visually-hidden">Todo form</legend>
    <div>
      <label for="todo">Add a ToDo</label>      
      <input bind:value={todo} type="text" id="todo" placeholder="new todo">
      <button onclick={addToDo}>
        <span>Add</span>
      </button>
    </div>
  </fieldset>
</form>


<style>
  fieldset {
    border:0;
    display: flex;

    padding:0;
  }
  div {
    display: flex;
    flex-flow: row wrap;
    gap:.5rem
  }
  label {
    flex-basis: 100%;
    font-weight: bold;
  }
  input {
    border:2px solid var(--color-blue)
  }
  button {
      all:unset;
      background:var(--color-green);
      display:flex;
      align-items:center;
      gap:.25rem;
      
  }
  
  input, button {
    padding:.25rem;
    font-size: .8rem;
    box-shadow:3px 3px 0 0 var(--color-blue);
    border-radius: .25rem;
    font-family: inherit;
    color: inherit
  }
</style>