<form action="/">
  <fieldset>
    <legend class="visually-hidden">Search form</legend>

    <div>
      <label for="query">Search the site</label>
      
      <input type="search" name="query" id="query" placeholder="enter keyword to search the site">
      <button>
        <span>Search</span>
        <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-search" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M10 10m-7 0a7 7 0 1 0 14 0a7 7 0 1 0 -14 0" /><path d="M21 21l-6 -6" /></svg>
      </button>
    </div>
  </fieldset>
</form>


<style>
  form {
    width: 100%;
    container-type: inline-size;
  }
  fieldset {
    border:0;
    display: flex;
    justify-content: end;
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
  button svg {
    width:1.25rem;
    fill: none;
    display:none
  }
  input, button {
    padding:.25rem;
    text-transform:uppercase;
    font-size: .8rem;
    box-shadow:3px 3px 0 0 var(--color-blue);
    border-radius: .25rem;
    font-family: inherit;
    color: inherit
  }

  @container (width < 11rem){
    label {
      display: none;
    }
    input[type='search'] {
      width: 4rem;
    }
    button > span {
      display: none;
    }
    button > svg {
      display: block;
    }
  }

  @container (width > 11rem) and (width < 14rem) {
    label {
      display: none;
    }
    input[type='search'] {
      width: 6rem;
    }
    button > svg {
      display: none;
    }
  }

  @container (width > 14rem) {
    div{
      width: 10rem;
    }
    input[type='search'] {
      width: 6rem;
    }
    
  }
  
  @container (width > 20rem) {
    div{
      width: 20rem;
    }
    input[type='search'] {
      width: 16rem;
    }
  }

  @container (width > 25rem) {
    div{
      width: 25rem;
    }
    input[type='search'] {
      width: 18rem;
    }
    button svg {
      display: block
    }
  }
</style>