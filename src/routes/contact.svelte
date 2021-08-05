<svelte:head>
	<title>Garrick Sewsankar | Contact</title>
	<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</svelte:head>

<script>
let sent = false;

const sendMessage = (e) =>{
	e.preventDefault();
	let nameValue = document.getElementById("name_id").value;
	let bodyValue = document.getElementById("body_id").value;
	if(nameValue === "" || bodyValue === ""){
		alert("Name or Body cannot be empty");
	}
	else if(sent === false){
		console.log({nameValue,bodyValue});
		sent = true;
	}
	else{
		alert("msg already sent");
	}
}
</script>

<style>
	.contact{
		padding: 1rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items:center;
		background-color: rgb(240, 240, 240);
	}

	.socials{
		display: flex;
		flex-direction: row;
		align-items: center;
		justify-content: center;
	}

	.socials i{
		padding: 10px;
		font-size: 3rem;
		color: lightgray;
	}

	
	.socials i:hover{
		color: rgb(100, 100, 100);
	}

	form{
		font-size: x-large;
	}

	.body{
		height: 150px;
		width: auto;
		box-sizing: border-box;
		border: 2px solid #ccc;
		border-radius: 4px;
		background-color: #f8f8f8;
		resize: none;
	}

	.name{
		height: auto;
		width: 150px;
		border: 2px solid #ccc;
		border-radius: 4px;
		background-color: #f8f8f8;
	}

	button{
		color: white;
		background-color: lightskyblue;
		border-radius: 20px;
		padding: 20px;
		font-size: large;
		border: lightskyblue;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	button:hover{
		cursor: pointer;
		background-color: rgb(106, 158, 190);
	}

	h4.show-msg{
		display: inline;
	}

	h4.hide{
		display: none;
	}

</style>

<h1>Contact</h1>

<div class="contact" id="contact">
	<div class="socials">
		<a href="https://www.facebook.com/profile.php?id=100009457129970&ref=bookmarks"target="_blank"><i class="fa fa-facebook"></i></a>
		<a href="https://twitter.com/gsewsankar31"target="_blank"><i class="fa fa-twitter"></i></a>
		<a href="https://www.instagram.com/gsewsankar/"target="_blank"><i class="fa fa-instagram"></i></a>
		<a href="https://www.youtube.com/thoughtsofgarrick"target="_blank"><i class="fa fa-youtube-play"></i></a>
		<a href="https://www.linkedin.com/in/garrick-sewsankar/"target="_blank"><i class="fa fa-linkedin"></i></a>
		<a href="https://www.github.com/gsewsankar"target="_blank"><i class="fa fa-github"></i></a>
	</div>
	<a href="Garrick Sewsankar Resume Fall 2021.pdf" target="_blank">View Current Resume</a>
	<div><i class="fa fa-phone"></i> (407)-797-6198 </div>
    <div><i class="fa fa-envelope"></i> gsewsankar@ufl.edu </div>
	<p>I programmed this to send a notification directly to my phone LOL. If you are here, send something!</p>
	<form>
		<label for="name">From:</label><br>
		<input type="text" placeholder="Your Name" id="name_id" name="name" class="name"><br>
		<label for="body">Body:</label><br>
		<textarea placeholder="Your Message" id="body_id" name="body" class="body"/>
	</form>
		<button on:click={sendMessage}>Send Now &nbsp;<i class="material-icons">send</i></button>
	<h4 class={sent ? "show-msg" : "hide"}>MESSAGE SENT</h4>

</div>

