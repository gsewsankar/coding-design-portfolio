<script>
	export let segment;

	function openNav() {
		document.getElementById("myNav").style.width = "100%";
	}

	function closeNav() {
		document.getElementById("myNav").style.width = "0%";
	}
</script>

<style>
.nav{
	display: flex;
	flex-direction: row;
	justify-content: center;
	align-items: center;
	padding: 1rem;
}

.topnav a:hover{
	color: limegreen;
}

.link{
	padding: 1rem;
	text-decoration: none;
	font-size: xx-large;
}

.active-link{
	padding: 1rem;
	font-size: xx-large;
	color: limegreen;
}

.home-btn img{
	height: 56px;
	width:auto;
}

.home-btn:hover{
	transform: scale(1.1);
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

	.nav .topnav{
		display: none;
	}

	.menu-btn{
		display: inline-block;
		text-decoration: none;
		max-height: 60px;
		font-size: xx-large;
	}

	.menu-btn:hover{
		cursor: pointer;
	}
}

.overlay {
  height: 100%;
  width: 0;
  position: fixed;
  z-index: 1;
  top: 0;
  left: 0;
  background-color: rgb(0,0,0);
  background-color: rgba(0,0,0, 0.9);
  overflow-x: hidden;
  transition: 0.5s;
}

.overlay-content {
  position: relative;
  top: 15%;
  width: 100%;
  text-align: center;
  margin-top: 30px;
}

.overlay a {
  padding: 8px;
  text-decoration: none;
  font-size: 36px;
  color: #818181;
  display: block;
  transition: 0.3s;
}

.overlay a:hover, .overlay a:focus {
  color: #f1f1f1;
}

.overlay .closebtn {
  position: absolute;
  top: 20px;
  right: 45px;
  font-size: 60px;
}

.overlay .closebtn {
  cursor: pointer;
}

@media screen and (max-height: 450px) {
  .overlay a {font-size: 20px}
  .overlay .closebtn {
  font-size: 40px;
  top: 15px;
  right: 35px;
  }
}

</style>

<nav class="nav" id="Nav">
	<a class="home-btn" href="." ><img src='logo-192.png' alt="brkn"></a>
	<div class="topnav">
		<a class={segment === "skills" ? "active-link" : "link"} href="skills" >Skills</a>
		<a class={segment === "experience" ? "active-link" : "link"} href="experience" >Experience</a>
		<a class={segment === "projects" ? "active-link" : "link"} href="projects" >Projects</a>
		<a class={segment === "education" ? "active-link" : "link"} href="education" >Education</a>
		<a class={segment === "contact" ? "active-link" : "link"} href="contact" >Contact</a>
	</div>
	<a href={segment} class="menu-btn" on:click={openNav}>&#9776;</a>
</nav>

<div id="myNav" class="overlay">
	<a href={segment} class="closebtn" on:click={closeNav}>&times;</a>
	<div class="overlay-content">
		<a href="." on:click={closeNav}>Home</a>
		<a href="skills" on:click={closeNav}>Skills</a>
		<a href="experience" on:click={closeNav} >Experience</a>
		<a href="projects" on:click={closeNav} >Projects</a>
		<a href="education" on:click={closeNav} >Education</a>
		<a href="contact" on:click={closeNav} >Contact</a>
	</div>
</div>
