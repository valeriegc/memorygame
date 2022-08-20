<script lang="ts">
	import Card from '$lib/Cards/Card.svelte';

	type Cards = { type: number; open: Boolean };
	let cards: Cards[] = [];
	let openCards: number[] = [];
	let pairCount = 0;

	for (let i = 0; i < 32; i++) {
		cards.push({ type: i % 16, open: false });
	}
	//shuffle array
	cards.sort(() => Math.random() - 0.5);

	function cardOpen(i: number) {
		if (openCards.length > 1) return;
		cards[i].open = true;
		openCards.push(i);
		if (openCards.length > 1) {
			cardCloser();
		}
	}

	function cardCloser() {
		let first = cards[openCards[0]];
		let second = cards[openCards[1]];
		openCards = [];
		if (first.type == second.type) {
			pairCount += 1;
		} else {
			setTimeout(() => {
				first.open = false;
				second.open = false;
				cards = [...cards];
			}, 2200);
		}
	}
</script>

<div class="grid">
	{#each cards as card, i}
		<div on:click={() => cardOpen(i)}>
			<Card {card} />
		</div>
	{/each}
</div>

<style>
	.grid {
		display: grid;
		grid-template-columns: repeat(8, 1fr);
		gap: 10px;
		width: 1200px;
	}
</style>
