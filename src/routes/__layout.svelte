<script>
	import Navigation from '../components/Navigation.svelte';
	import TuneGrid from '../components/TuneGrid.svelte';
</script>

<main>
	<Navigation />
	<TuneGrid>
		<slot />
	</TuneGrid>
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
</style>
