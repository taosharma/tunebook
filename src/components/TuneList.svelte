<script>
	import tunebook from '../../data/tunebook';
	import { dndzone } from 'svelte-dnd-action';

	function handleSort(e) {
		items = e.detail.items;
	}

	let items = [...tunebook];
</script>

<section use:dndzone={{ items }} on:consider={handleSort} on:finalize={handleSort}>
	{#each items as item (item.orderId)}
		<div>{item.name}</div>
	{/each}
</section>

<style>
	section {
		height: 60vh;
		width: 25vw;
		background-color: blue;
	}
</style>
