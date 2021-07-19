<script>
	import Nav from '../components/Nav.svelte';
	export let segment;
</script>

<style>
	.app{
		background-color: white;
		min-height: 100vh;
	}
	main{
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}
	.footer{
		left: 0;
		bottom: 0;
		width: 100%;
		height: 100px;
		background-color: lightgrey;
		color: gray;
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>

<div class="app">
<Nav {segment}/>

<main>
	<slot></slot>
</main>
</div>
<div class="footer">
	© 2021 A Garrick Website. All rights reserved.
</div>

