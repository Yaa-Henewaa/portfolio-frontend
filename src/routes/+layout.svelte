<script lang="ts">
	import '../app.css';
	import Navbar from "./(main)/components/navbar.svelte"
	let { children } = $props();
</script>


<Navbar/>
{@render children()}
