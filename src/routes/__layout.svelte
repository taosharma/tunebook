<script>
	import Navigation from '../components/Navigation.svelte';
</script>

<main>
	<Navigation />
	<section class="tune-grid">
		<div class="center-left container" />
		<div class="center-right container" />
		<div class="center">
			<slot />
		</div>
		<div class="center-top container" />
		<div class="center-bottom container" />
	</section>
</main>

<style>
	main {
		height: 100vh;
		width: 100vw;
		display: flex;
		align-items: center;
		justify-content: center;
		background-color: cornflowerblue;
	}
	.tune-grid {
		display: grid;
		grid-template-columns: 5vw 25vw 5vw;
		grid-template-rows: 5vh 60vh 5vh;
		align-items: center;
		justify-items: center;
		background-color: crimson;
	}

	.center-left {
		grid-area: 2 / 1 / 2 / 1;
	}

	.center-right {
		grid-area: 2 / 3 / 2 / 3;
	}

	.center-top {
		grid-area: 1 / 2 / 1 / 2;
	}

	.center-bottom {
		grid-area: 3 / 2 / 3 / 2;
	}

	.center {
		grid-area: 2 / 2 / 2 / 2;
	}

	.container {
		height: 0.5em;
		width: 0.5em;
		border: 0.1em solid black;
	}
</style>
