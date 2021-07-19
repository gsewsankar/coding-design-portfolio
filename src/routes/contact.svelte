<svelte:head>
	<title>Garrick Sewsankar | Contact</title>
	<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
</svelte:head>

<script>
let sent = false;

const sendMessage = () =>{
	sent = !sent;
}
</script>

<style>
	form{
		font-size: x-large;
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

<div id="contact">
	<p>I programmed this to send a notification directly to my phone LOL. If you are here, send something!</p>
	<form>
		<label for="name">From:</label><br>
		<input type="text" placeholder="Your Name" id="name" name="name"><br>
		<label for="body">Body</label><br>
		<input type="text" placeholder="Your Message" id="body" name="body">
	</form>
	<button on:click={sendMessage}>Send Now &nbsp;<i class="material-icons">send</i></button>
	<h4 class={sent ? "show-msg" : "hide"}>MESSAGE SENT</h4>
</div>

