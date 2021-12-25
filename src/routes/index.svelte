<script>
	import { Transition, Sheet } from '$lib';

	let open = false;
</script>

<button on:click={() => open = !open}>toggle</button>


	<Sheet open={open}>
		<div class="w-60 p-10 bg-gray-50 rounded-r-xl my-auto">
			hoi
		</div>
	</Sheet>
