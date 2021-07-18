<script>
	export let segment;

	let collapse = true;

	function toggleNav(){
		collapse = !collapse;
	}
</script>

<style>
	.nav{
		display: flex;
		flex-direction: row;
		justify-content: center;
		padding: 1rem;
	}

	.nav .dropdown{
		padding: 1rem;
	}

	.link{
		padding: 1rem;
		text-decoration: none;
	}

	.active-link{
		padding: 1rem;
		color: rgb(73, 168, 81);
	}

	.menu-btn{
		padding: 1rem;
		text-decoration: none;
		display: none;
	}

	.menu-btn:hover{
			cursor: pointer;
	}

	@media only screen and (max-width: 600px) {
		.nav{
			justify-content: space-between;
		}
		
		.nav .dropdown-close{
			display: none;
		}

		.nav .dropdown-open{
			display: flex;
			flex-direction: column;
			padding: 0rem 3rem;
		}

		.menu-btn{
			display: inline-block;
			text-decoration: none;
			max-height: 60px;
		}

		.menu-btn:hover{
			cursor: pointer;
		}
	}

</style>

<nav class="nav" id="Nav">
	<a class={segment === undefined ? "active-link" : "link"} href="." >GS</a>
	<div class="dropdown">
		<div class={collapse ? "dropdown-close" : "dropdown-open"}>
			<a class={segment === "skills" ? "active-link" : "link"} href="skills" on:click={toggleNav}>Skills</a>
			<a class={segment === "experience" ? "active-link" : "link"} href="experience" on:click={toggleNav} >Experience</a>
			<a class={segment === "projects" ? "active-link" : "link"} href="projects" on:click={toggleNav} >Projects</a>
			<a class={segment === "education" ? "active-link" : "link"} href="education" on:click={toggleNav} >Education</a>
			<a class={segment === "contact" ? "active-link" : "link"} href="contact" on:click={toggleNav} >Contact</a>
		</div>
	</div>
	<a href={segment} class="menu-btn" on:click={toggleNav}>&#9776;</a>
</nav>
