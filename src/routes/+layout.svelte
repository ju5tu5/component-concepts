<script>
	import '$lib/assets/style.css'
	import favicon from '$lib/assets/favicon.svg'
	import { Header, Nav } from "$lib/index.js"

	let { children } = $props()
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<Header/>

{@render children()}

<footer>
	<p><span>&copy;</span> Copyleft, all wrongs reversed.</p>
</footer>

<style>
	footer span {
		display: inline-block;
		margin: 0; padding: 0;
		transform-origin: 55% 52%;
		transform: rotate(180deg);
	}
</style>