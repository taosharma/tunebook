<script>
	import Navigation from '../components/Navigation.svelte';
</script>

<main>
	<Navigation />
	<section class="tune-grid">
		<div class="center-left button" />
		<div class="center-top button" />
		<div class="center">
			<slot />
		</div>
		<div class="center-bottom button" />
		<div class="center-right button" />
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
		grid-template-columns: 2.5em 35vw 2.5em;
		grid-template-rows: 2.5em 70vh 2.5em;
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

	.button {
		height: 0.5em;
		width: 0.5em;
		border: 0.1em solid black;
	}
</style>
