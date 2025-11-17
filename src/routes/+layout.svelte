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
	<Nav/>
</footer>