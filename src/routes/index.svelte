<svelte:head>
	<title>Garrick Sewsankar</title>
</svelte:head>

<script>
import { onMount } from 'svelte';
import Skills from './skills.svelte';
import Experience from './experience.svelte';
import Projects from './projects.svelte';
import Education from './education.svelte';
import Contact from './contact.svelte';

let mybutton;

onMount(() => {
	mybutton = document.getElementById("myBtn");
	// When the user scrolls down 20px from the top of the document, show the button
	window.onscroll = function() {scrollFunction()};

	function scrollFunction() {
		if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
			mybutton.style.display = "block";
		} else {
			mybutton.style.display = "none";
		}
		}
	});
	// When the user clicks on the button, scroll to the top of the document
	function topFunction() {
		document.body.scrollTop = 0;
		document.documentElement.scrollTop = 0;
	}

</script>

<style>
	.index{
		width: 100%;
		background: url('../uf.jpg') no-repeat center;
		background-size: cover;
		background-attachment: fixed;
	}
	.top{
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;;
		animation-name: floating;
		animation-duration: 3s;
		animation-iteration-count: infinite;
		animation-timing-function: ease-in-out;
	}

	.glass{
		padding: 2rem;
		background-color: rgba(255, 255, 255, 0.808);
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.home{
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
	}

	h3{
		padding: 1rem;
	}

	.scrollUp {
		display: none;
		position: fixed;
		bottom: 20px;
		right: 30px;
		z-index: 99;
		font-size: 18px;
		border: none;
		outline: none;
		background-color: rgba(109, 109, 109, 0.829);
		color: white;
		cursor: pointer;
		padding: 15px;
		border-radius: 4px;
	}

	.scrollUp:hover {
		background-color:rgba(143, 143, 143, 0.89);
	}

	@keyframes floating {
		0% { transform: translate(0,  0px); }
		50%  { transform: translate(0, 15px); }
		100%   { transform: translate(0, -0px); }
	}

	.newly-added {
		animation: flyin 1.2s ease forwards;
		opacity: 0;
		transform: scale(2);
		filter: blur(4px);
	}

	@keyframes flyin {
		to { 
			filter: blur(0);
			transform: scale(1);
			opacity: 1;
		}
	}

	@media only screen and (max-width: 600px) {
		h3{
			padding-top: 50px;
			text-align: center;
		}
	}
</style>

<div class="home">
<div class="index" id="index">
<div class="glass">
	<div class="top">
	<h1>Hi I'm Garrick Sewsankar...</h1>
	<img class="newly-added" src=https://i.ibb.co/xSPkS8y/small.jpg alt=pfp />
	</div>
	<h3 class="newly-added">Software Engineer - Web Developer - UI/UX Designer<br> Philosopher - YouTuber - Start-Up Founder <br> Entrepreneur - Businessman - CEO </h3>
</div>
</div>
<Skills/>
<Experience/>
<Projects/>
<Education/>
<Contact/>
<button on:click={topFunction} id="myBtn" class="scrollUp" title="Go to top">Top</button>
</div>
