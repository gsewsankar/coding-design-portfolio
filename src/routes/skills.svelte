<svelte:head>
	<title>Garrick Sewsankar | Skills</title>
</svelte:head>

<script>

</script>

<style>

	h1{
		color: white;
	}

	.skills{
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		background-color: rgb(80, 80, 80);
	}

	.cards{
		display: flex;
		justify-content: center;
		flex-wrap: wrap;
	}

	.item{
		padding:1rem;
		animation: flyin 1.2s ease forwards;
		opacity: 0;
		transform: scale(2);
		filter: blur(4px);
	}

	.item img{
		width: auto;
		height: 200px;
	}

	@keyframes flyin {
		to { 
			filter: blur(0);
			transform: scale(1);
			opacity: 1;
		}
	}

</style>

<div class="skills">
<h1>My Skills</h1>

<div class=cards>
	<div class="item">
		<img src="https://upload.wikimedia.org/wikipedia/commons/1/18/ISO_C%2B%2B_Logo.svg" alt="brkn" />
	</div>
	<div class="item">
		<img src="https://seeklogo.com/images/J/java-logo-7833D1D21A-seeklogo.com.png" alt="brkn" />
	</div>
	<div class="item">
		<img src="https://miro.medium.com/max/500/1*cPh7ujRIfcHAy4kW2ADGOw.png" alt="brkn" />
	</div>
	<div style="background-color: lightgrey;" class="item">
		<img src="https://firebase.google.com/downloads/brand-guidelines/PNG/logo-vertical.png" alt="brkn" />
	</div>
	<div class="item">
		<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/17/GraphQL_Logo.svg/768px-GraphQL_Logo.svg.png" alt="brkn" />
	</div>
	<div class="item">
		<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/Svelte_Logo.svg/747px-Svelte_Logo.svg.png" alt="brkn" />
	</div>
	<div class="item">
		<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/1200px-HTML5_logo_and_wordmark.svg.png" alt="brkn" />
	</div>
	<div class="item">
		<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/CSS3_logo_and_wordmark.svg/1200px-CSS3_logo_and_wordmark.svg.png" alt="brkn" />
	</div>
	<div class="item">
		<img src="https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png" alt="brkn" />
	</div>
	<div class="item">
		<img src=https://thumbs.gfycat.com/SandySinfulBullfrog-size_restricted.gif alt="brkn" />
	</div>
	<div class="item">
		<img src="https://i2.wp.com/allhtaccess.info/wp-content/uploads/2018/03/programming.gif?fit=1281%2C716&ssl=1" alt="brkn" />
	</div>
	
</div>

</div>