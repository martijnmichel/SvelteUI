<script lang="ts">
	export let position = 'left';
	export let open = false;
	export let width = 100
	export let height = 400
</script>


<div class="fixed transition-all flex" style="height: {height}px; top: 50vh; margin-top: -{height/2}px" class:open data-position={position}>

	<slot/>
</div>

<style>

	[data-position="left"] {
		left: 0;
		transform: translate(-100vw,0);
	}

	[data-position="bottom"] {
		left: 0;
		right: 0;
		bottom: 0;
		transform: translate(0,100vh)
	}

	.open {
		transform: translate(0,0)
	}
</style>