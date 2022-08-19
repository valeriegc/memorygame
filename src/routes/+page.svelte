<script lang="ts">
	import Button from '$lib/Button.svelte';
	import Backside from '$lib/Cards/Backside.svelte';

	type Cards = { type: Number; open: Boolean };
	let cards: Cards[] = [];

	for (let i = 0; i < 32; i++) {
		cards.push({ type: i % 16, open: false });
	}
</script>

<div class="wrap">
	<div class="grid">
		{#each cards as card}
			<Backside />
		{/each}
	</div>
</div>

<style>
	.grid {
		display: grid;
		grid-template-columns: repeat(8, 1fr);
		gap: 10px;
		width: 1200px;
	}
	.wrap {
		display: flex;
		align-items: flex-end;
		justify-content: center;
		height: 100vh;
		margin-bottom: 2%;
	}
</style>
