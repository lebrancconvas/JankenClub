<script lang="ts">
	import JankenCard from '../components/JankenCard.svelte';

	let isLoggedin: boolean = false;
</script>

<svelte:head>
	<title>Janken Club</title>
</svelte:head>

<main>
	<header>
		<div>
			<h1>Janken Club</h1>
		</div>
	</header>
	{#if isLoggedin}
		<section id="canvas">
				<JankenCard hand="Rock" img="https://cdn-icons.flaticon.com/png/512/3562/premium/3562093.png?token=exp=1660465425~hmac=8f546422a5c6a4f52b3619a6a4682964" />
				<JankenCard hand="Paper" img="https://cdn-icons-png.flaticon.com/512/2910/2910908.png" />
				<JankenCard hand="Scissors" img="https://cdn-icons.flaticon.com/png/512/4151/premium/4151732.png?token=exp=1660465628~hmac=83d19677fb272fc38e456ac4b52f2546" />
		</section>
	{:else}
		<section id="canvas-not">
			<div>
				<h1>You don't have an access to the website</h1>
			</div>
		</section>
	{/if}
</main>

<style>
	* {
		font-family: 'Bungee', cursive;
	}

	header {
		text-align: center;
		margin: 10px;
		font-size: 25px;
	}

	#canvas {
		/* border: 2px solid black; */
		display: grid;
		grid-template-columns: 40% 40% 40%;
		text-align: center;
		margin: 0 auto;
	}

	#canvas-not {
		text-align: center;
	}
</style>