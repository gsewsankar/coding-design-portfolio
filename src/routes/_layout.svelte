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
	.fullscreen-video-wrap{
		position:absolute;
		top:0;
		left:0;
		width:100%;
		height:100vh;
		overflow:hidden;
		z-index: -1;
	}
  
  .fullscreen-video-wrap video{
    min-height:100%;
    min-width:100%;
	z-index: -1;
	filter: opacity(0.5);
  }
</style>

<div class="app">

<div class="fullscreen-video-wrap"><video src="bg.mp4" autoplay loop muted></video></div>

<Nav {segment}/>

<main>
	<slot></slot>
</main>

</div>
