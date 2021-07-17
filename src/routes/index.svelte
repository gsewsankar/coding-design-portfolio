<svelte:head>
	<title>Garrick Sewsankar</title>
</svelte:head>

<script>

</script>

<style>
	.top{
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;
		animation-name: floating;
		animation-duration: 3s;
		animation-iteration-count: infinite;
		animation-timing-function: ease-in-out;
	}

	h3{
		padding: 1rem;
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
</style>

<div id="index">
	<div class="top">
	<h1>Hi I'm Garrick Sewsankar...</h1>
	<img class="newly-added" src=https://i1.wp.com/i.pinimg.com/236x/ce/2a/95/ce2a95e99faceaf7af19c273b10ebcc1.jpg alt=pfp />
	</div>
	<h3 class="newly-added">"Aspiring"<br>Software Engineer - Web Developer <br> Philosopher - YouTuber - Start-Up Founder <br> Entrepreneur - Businessman - CEO </h3>
	
</div>
