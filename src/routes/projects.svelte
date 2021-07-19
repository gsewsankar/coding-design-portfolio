<svelte:head>
	<title>Garrick Sewsankar | Projects</title>
</svelte:head>

<script>

</script>

<style>
.projects{
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
}
.card{
	display: flex;
	margin: 1rem;
	flex-direction: column;
	border: 2px solid rgb(0, 57, 95);
	border-radius: 5px;
}

.card:hover{
	transform: scale(1.05);
	cursor: pointer;
}

.card p{
	padding: 2rem;
	border-top: 1px solid rgb(0, 57, 95);
}

@media only screen and (max-width: 600px) {
	.card img{
		width: 300px;
	}
}

</style>

<h1> Projects </h1>

<div class="projects" id="projects">
	<div class="card">
		<img width=500px height="auto" src="fwee_logo.svg" alt=brkn>
		<p>This project is about this and that</p>
	</div>
	<div class="card">
		<img width=500px height="auto" src="drive.PNG" alt=brkn>
		<p>This project is about this and that</p>
	</div>
	<div class="card">
		<img width=500px height="auto" src="eds.PNG" alt=brkn>
		<p>This project is about this and that</p>
	</div>
	<div class="card">
		<img width=500px height="auto" src="wlx.PNG" alt=brkn>
		<p>This project is about this and that</p>
	</div>
	<div class="card">
		<img width=500px height="auto" src="blog.PNG" alt=brkn>
		<p>This project is about this and that</p>
	</div>
	<div class="card">
		<img width=500px height="auto" src="gitsite.PNG" alt=brkn>
		<p>This project is about this and that</p>
	</div>
</div>