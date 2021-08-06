<script>
	import Nav from '../components/Nav.svelte';
	export let segment;
	import { onMount } from 'svelte';
	import firebase from 'firebase/app';
	import 'firebase/firestore';
	const firebaseConfig = {
	apiKey: "AIzaSyDuSiEXG-ZOyFLlxQ1UniEyKKXCLT-ym30",
	authDomain: "message-sender-8c7f0.firebaseapp.com",
	projectId: "message-sender-8c7f0",
	storageBucket: "message-sender-8c7f0.appspot.com",
	messagingSenderId: "335037389016",
	appId: "1:335037389016:web:3d336f13d92368c6671fad",
	measurementId: "G-CELWL9K1JQ"
	};
	onMount(() => {
		firebase.initializeApp(firebaseConfig);
	});
</script>

<style>
	.app{
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
		padding-top: 1rem;
		padding-bottom: 1rem;
		flex-direction: column;
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
	<p>I made this site with <a href=https://sapper.svelte.dev target="_blank" rel="noopener noreferrer">Svelte Sapper</a></p>
	<p>© 2021 A Garrick Website. All rights reserved.</p>
</div>

