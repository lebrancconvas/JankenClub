<script lang="ts">

</script>

<svelte:head>
	<title>Login | Janken Club</title>
</svelte:head>

<main>
	<header>
		<div>
			<h1>Login</h1>
		</div>
	</header>
	<section id="login-canvas">
		<div id="login-card">
			<form action="">
				<label for="">Username</label>
				<br>
				<input type="text" name="username" id="login-username">
				<br>
				<button type="submit">Login</button>
			</form>
		</div>
	</section>
</main>

<style>
	* {
		font-family: "Bungee", cursive;
	}

	header {
		text-align: center;
	}

	#login-canvas {
		/* border: 2px solid red; */
		height: 500px;
	}

	#login-card {
		border: 2px solid black;
		height: 80%;
		width: 50%;
		margin: 10px auto; 
		padding: 10px; 
		border-radius: 10px;
		box-shadow: 1px 1px 1px 1px black;
		text-align: center;
		background-color: rgb(255,192,96);
		background-color: linear-gradient(90deg, rgba(255,192,96,1) 37%, rgba(228,178,50,1) 80%);
	}

	label {
		font-size: 30px;
		margin: 20px;
	}

	input {
		font-size: 23px;
		outline: 0;
		border-width: 0 0 2px;
	}

	button {
		margin: 10px 0;
	}
</style>