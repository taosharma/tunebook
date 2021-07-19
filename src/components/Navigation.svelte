<script>
	//TODO: Make spaces between even - maybe by dividing unused container space evenly between all sides of items in container.
	import Header from './Header.svelte';
</script>

<section class="navigation-container">
	<div class="header" />
	<div class="view-control" />
	<div class="tune-type-control" />
	<div class="audio-control" />
</section>

<style>
	.navigation-container {
		height: 60vmin;
		width: 40vmin;
		margin: 1em;
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		align-items: center;
		justify-content: center;
		background-color: greenyellow;
	}

	.header {
		height: 10vmin;
		width: 37.5vmin;
		border: 0.1em solid black;
	}

	.audio-control {
		height: 10vmin;
		width: 37.5vmin;
		border: 0.1em solid black;
	}

	.view-control {
		height: 30vmin;
		width: 10vmin;
		margin-right: 1.25vmin;
		border: 0.1em solid black;
	}

	.tune-type-control {
		height: 30vmin;
		width: 20vmin;
		margin-left: 1.25vmin;
		border: 0.1em solid black;
	}
</style>
