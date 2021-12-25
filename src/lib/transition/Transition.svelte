<script lang="ts">
import { fly } from "svelte/transition";

    export let open = false;
    export let enter = undefined;
    export let leave = undefined;
</script>

{#if open}
    <div in:fly={enter} out:fly={leave}>
        <slot  />
    </div>
{/if}