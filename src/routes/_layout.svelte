<script>
	import Nav from '../components/Nav.svelte';
	export let segment;
</script>

<style>
	main{
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>

<Nav {segment}/>

<main>
	<slot></slot>
</main>