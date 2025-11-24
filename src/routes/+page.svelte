<script>
  import { FdndLogo, SearchForm, Todo, List, TodoForm } from "$lib"
  	
    // let listItems = ["Hello", "World"];
    let listItems = $state(["Hello", "World"]);
    
</script>

<h2>Goede voorbeelden</h2>

<ul>
  <li><a href="https://vsheo.github.io/i-love-web/CSS-color-generator/">https://vsheo.github.io/i-love-web/CSS-color-generator/</a></li>
  <li><a href="https://github.com/fdnd-agency/bijlmerchronicles/blob/901b3e5f6bf30170c62ff60719127621fd49a292/src/lib/components/HamburgerMenu.svelte#L45">https://github.com/fdnd-agency/bijlmerchronicles/blob/901b3e5f6bf30170c62ff60719127621fd49a292/src/lib/components/HamburgerMenu.svelte#L45</a></li>
  <li><a href="https://github.com/fdnd-agency/oncollaboration/blob/organisme-filters/src/lib/atoms/Select.svelte">https://github.com/fdnd-agency/oncollaboration/blob/organisme-filters/src/lib/atoms/Select.svelte</a></li>
</ul>


<h2>Two way binding</h2>

<!-- <List bind:listItems />
<TodoForm bind:listItems />
 -->

<Todo bind:listItems />

<hr>
<h2>A long-expected party</h2>
<p>When Mr. Bilbo Baggins of Bag End announced that he would shortly be celebrating his eleventy-first birthday with a party of special magnificence, there was much talk and excitement in Hobbiton.</p>
<p>;) Joost</p>

<div>
  <SearchForm />
</div>

<SearchForm />

<div>
<FdndLogo>
<h3>Dit is een test</h3>
</FdndLogo>
</div>

<style>
  div {
    width: 12rem;
  }
</style>