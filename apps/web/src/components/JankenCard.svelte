<script lang="ts">
	export let hand: string;
	export let img: string;

	const handleClick = (): void => {
		alert(`You selected ${hand}`);
	};
</script>

<main>
	<div id="card-janken" on:click={handleClick}>
		<div id="card-img">
			<img src={img} alt={hand}>
		</div>
		<div id="card-name">
			{hand}
		</div>
	</div>
</main>

<style>
	#card-janken {
		border: 2px solid black;
		width: 27%;
		height: 100%;
		text-align: center;
		padding: 10px;
		border-radius: 10px;
		box-shadow: 1px 1px 1px 1px black;
		background-color: rgb(36, 170, 36);
		cursor: pointer;
		margin: 20px;
	}

	img {
		width: 128px;
		height: 128px;
	}

	#card-janken:active {
		transform: scale(0.98);
	}

	#card-name {
		margin-top: 20px;
		font-size: 30px;
	}
</style>