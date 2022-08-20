<script lang="ts">
	import Backside from './Backside.svelte';
	import Frontside from './Frontside.svelte';
	import Cat from './Pictures/Cat.svelte';
	import Dog from './Pictures/Dog.svelte';
	import Panda from './Pictures/Panda.svelte';
	import Horse from './Pictures/Horse.svelte';
	import Elephant from './Pictures/Elephant.svelte';
	import Zebra from './Pictures/Zebra.svelte';
	import Rhino from './Pictures/Rhino.svelte';
	import Sheep from './Pictures/Sheep.svelte';
	import Rabbit from './Pictures/Rabbit.svelte';
	import Whale from './Pictures/Whale.svelte';
	import Penguin from './Pictures/Penguin.svelte';
	import Monkey from './Pictures/Monkey.svelte';
	import Fish from './Pictures/Fish.svelte';
	import Fox from './Pictures/Fox.svelte';
	import Shark from './Pictures/Shark.svelte';
	import Snake from './Pictures/Snake.svelte';

	export let card: { type: number; open: Boolean };

	let cardThemes = [
		Panda,
		Horse,
		Elephant,
		Zebra,
		Rhino,
		Sheep,
		Rabbit,
		Whale,
		Cat,
		Penguin,
		Monkey,
		Fish,
		Fox,
		Shark,
		Snake,
		Dog
	];
</script>

{#if card.open == true}
	<Frontside>
		<svelte:component this={cardThemes[card.type]} />
	</Frontside>
{:else}
	<Backside />
{/if}
