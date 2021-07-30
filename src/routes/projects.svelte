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
		<a href="https://github.com/gsewsankar/fwee-dev" target="_blank" rel="noopener noreferrer">
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
				Programmed a data visualization dashboard 
				using a dataset for car accidents across 
				the United States from 2016-2021. Designed complex 
				trend queries to perform trend analysis on factors 
				that affect car accidents over time. 
				<b>(Oracle SQL, React, ChartJS)</b>
				</p>
			</div>
		</a>
		<a href="description.pdf" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="eds.PNG" alt=brkn>
				<h3><b>Event Driven Simulation of Network Cache</b></h3>
				<p> 
				Designed, and Developed an event driven simulation
				for a project related to Probablility in Computer Science
				and Machine Learning. The simulation allowed a user
				to select a cache replacement policy out of 4 options,
				then would return statistics related to the completion time.
				Results could be used to analyze which cache replacement policies 
				worked best and under what scenarios. 
				<b>(C++)</b>
				</p>
			</div>
		</a>
		<a href="https://www.watchlistexchange.com" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="wlx.PNG" alt=brkn>
				<h3><b>WatchList Exchange</b></h3>
				<p> 
				Implemented a search system where users can query
				a stock ticker and recieve its current price. The idea
				is to allow users to create and share custom stock watchlists. 
				Utilized Amazon Web Sevices such as Cognito, S3 Bucket, DynamoDB, 
				and Amplify.
				<b>(React, AWS, Serverless)</b>
				</p>
			</div>
		</a>
		<a href="https://digital-literacy-garrick.netlify.app" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="blog.PNG" alt=brkn>
				<h3><b>Thoughts of Garrick Blog</b></h3>
				<p> 
				Designed and built a Blog where I share my thoughts and Life Philosophy.
				Allows me to share my thoughts into words, words into actions, actions into
				habits, habits into character, and character into destiny. Encourages people 
				to look inward to discover how they can become the best they can be. Also,
				discusses topics relating to the future of the world and society. 
				<b>(React, CSS, ThreeJS)</b>
				</p>
			</div>
		</a>
		<a href="https://gsewsankar.github.io" target="_blank" rel="noopener noreferrer">
			<div class="card">
				<img width=500px height="auto" src="gitsite.PNG" alt=brkn>
				<h3><b>Github Website</b></h3>
				<p> 
				This is my old archived website. I made this with pure html, css, and
				javascript. I will eventually get around to redesigning it into
				links to my other websites, like a linktree. 
				<b>(HTML, CSS, Javascript)</b>
				</p>
			</div>
		</a>
	</div>
</div>