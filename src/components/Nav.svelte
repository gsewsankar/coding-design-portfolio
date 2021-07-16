<script>
	export let segment;
</script>

<style>
	.nav{
		display: flex;
		flex-direction: row;
		justify-content: center;
		padding: 1rem;
	}

	.link{
		padding: 1rem;
	}

	.active-link{
		padding: 1rem;
		color: purple;
	}
</style>

<div class="nav" id="Nav">
	<a class={segment === undefined ? "active-link" : "link"} href="." >Home</a>
	<a class={segment === "skills" ? "active-link" : "link"} href="skills" >Skills</a>
	<a class={segment === "experience" ? "active-link" : "link"} href="experience" >Experience</a>
	<a class={segment === "projects" ? "active-link" : "link"} href="projects" >Projects</a>
	<a class={segment === "education" ? "active-link" : "link"} href="education" >Education</a>
	<a class={segment === "contact" ? "active-link" : "link"} href="contact" >Contact</a>
</div>
