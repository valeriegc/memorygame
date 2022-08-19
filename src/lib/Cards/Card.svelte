<script lang="ts">
	import Backside from './Backside.svelte';
	import Frontside from './Frontside.svelte';
	export let cardActive: Boolean;
</script>

{#if cardActive == true}
	<Frontside />
{:else}
	<Backside />
{/if}

<style>
</style>
