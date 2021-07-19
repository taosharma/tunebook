<section class="tune-grid">
	<div class="center-left button" />
	<div class="center-top button" />
	<div class="center-panel">
		<slot />
	</div>
	<div class="center-bottom button" />
	<div class="center-right button" />
</section>

<style>
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

	.center-panel {
		grid-area: 2 / 2 / 2 / 2;
	}

	.button {
		height: 0.5em;
		width: 0.5em;
		border: 0.1em solid black;
	}
</style>
