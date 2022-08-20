<script>
	import Frontside from '$lib/Cards/Frontside.svelte';
	import Panda from '$lib/Cards/Pictures/Panda.svelte';
</script>

<div class="wrap">
	<Frontside><Panda /></Frontside>
</div>

<style>
	.wrap {
		display: flex;
		align-items: center;
		justify-content: center;
		height: 100vh;
	}
</style>
