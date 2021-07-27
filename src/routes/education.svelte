<svelte:head>
	<title>Garrick Sewsankar | Education</title>
</svelte:head>

<script>

</script>

<style>
.education{
	display: flex;
	flex-direction: row;
	justify-content: space-between;
}

.left{
	padding-right: 100px;
	display: flex;
	flex-direction: column;
	align-items: flex-start;
}

.right{
	display: flex;
	flex-direction: column;
}

h2{
	font-size: 2rem;
}

@media only screen and (max-width: 600px) {
	.education{
		display: flex;
		flex-direction: column;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;
		padding-left: 20px;
		padding-right: 20px;
	}
	.education img{
		width: 300px;
		height: auto;
	}
	.left{
		padding-right: 0;
		text-align: center;
		align-items: center;
	}
	.left ul{
		text-align: left;
	}
}
</style>

<h1>Education</h1>

<div class="education" id="education">
	<div class="left">
		<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8e/University_of_Florida_logo.svg/396px-University_of_Florida_logo.svg.png" alt="brkn">
		<h2 class="major">Bachelor of Science in Computer Science</h2>
		<h2>May 2022</h2>
		<h3>Significant Courses</h3>
		<ul>
			<li>Data Structures and Algorithms</li>
			<li>Probability in Computer Science for Machine Learning</li>
			<li>Ethics, Data, and Technology</li>
			<li>Business Law</li>
		</ul>
	</div>
	<div class="right">
		<img width=500px height="auto" src="https://upload.wikimedia.org/wikipedia/en/thumb/1/14/Florida_Gators_gator_logo.svg/1280px-Florida_Gators_gator_logo.svg.png" alt="brkn">
		<img width=500px height="auto" src="uf.jpg" alt=brkn>
	</div>
</div>