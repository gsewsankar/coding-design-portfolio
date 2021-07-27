<svelte:head>
	<title>Garrick Sewsankar | Projects</title>
</svelte:head>

<script>

</script>

<style>
.projects{
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
}
.cards{
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
}

a{
	text-decoration: none;
	display: flex;
	flex-wrap: wrap;
	justify-content: center;
}

.card{
	display: flex;
	margin: 1rem;
	flex-direction: column;
	justify-content: flex-start;
	align-items: center;
	border: 2px solid rgb(0, 57, 95);
	border-radius: 5px;
	background-color: white;
}

.card:hover{
	transform: scale(1.05);
	cursor: pointer;
}

.card img{
	border-bottom: 1px solid rgb(0, 57, 95);
}

.card p{
	max-width: 400px;
	text-align: center;
}

.card h3{
	margin: 0 auto;
	max-width: 450px;
	text-align: center;
}

@media only screen and (max-width: 600px) {
	.card img{
		width: 300px;
	}

	.card p{
		max-width: 200px;	
	}

	.card h3{
		margin: 0 auto;
		max-width: 280px;
		text-align: center;
	}
}

</style>

<div class="projects" id="projects">
 <h1> Projects </h1>
	<div class="cards">
		<a href="https://www.watchlistexchange.com" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="fwee_logo.svg" alt=brkn>
				<h3><b>Free World Exchange</b></h3>
				<p> 
				Created, Designed, and Developed a fully 
				functional online Social Media Marketplace 
				where users exchange virtual items using 
				an in-market digital currency backed by time. 
				<b>(React, React Native, Firebase, GraphQL)</b>
				</p>
			</div>
		</a>
		<a href="https://github.com/chensation/Auto-Accident-Trend-Analysis-Tool" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="drive.PNG" alt=brkn>
				<h3><b>Auto Accident Data Visualization Tool</b></h3>
				<p> 
				Created, Designed, and Developed a fully 
				functional online Social Media Marketplace 
				where users exchange virtual items using 
				an in-market digital currency based on time. 
				<b>(Oracle SQL, React)</b>
				</p>
			</div>
		</a>
		<a href="description.pdf" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="eds.PNG" alt=brkn>
				<h3><b>Event Driven Simulation of Network Cache</b></h3>
				<p> 
				Created, Designed, and Developed a fully 
				functional online Social Media Marketplace 
				where users exchange virtual items using 
				an in-market digital currency based on time. 
				<b>(C++)</b>
				</p>
			</div>
		</a>
		<a href="https://www.watchlistexchange.com" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="wlx.PNG" alt=brkn>
				<h3><b>WatchList Exchange</b></h3>
				<p> 
				Created, Designed, and Developed a fully 
				functional online Social Media Marketplace 
				where users exchange virtual items using 
				an in-market digital currency based on time. 
				<b>(React, AWS, Serverless)</b>
				</p>
			</div>
		</a>
		<a href="https://digital-literacy-garrick.netlify.app" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="blog.PNG" alt=brkn>
				<h3><b>Thoughts of Garrick Blog</b></h3>
				<p> 
				Created, Designed, and Developed a fully 
				functional online Social Media Marketplace 
				where users exchange virtual items using 
				an in-market digital currency based on time. 
				<b>(React, CSS, ThreeJS)</b>
				</p>
			</div>
		</a>
		<a href="https://gsewsankar.github.io" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="gitsite.PNG" alt=brkn>
				<h3><b>Github Website</b></h3>
				<p> 
				Created, Designed, and Developed a fully 
				functional online Social Media Marketplace 
				where users exchange virtual items using 
				an in-market digital currency based on time. 
				<b>(HTML, CSS, Javascript)</b>
				</p>
			</div>
		</a>
	</div>
</div>