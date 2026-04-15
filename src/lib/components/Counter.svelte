<script>
    import { json } from "@sveltejs/kit";

    let props = $props();
    // con proprs andiamo ad accedere a un oggetto di js e poi lo sostituiamo sotto al posto dello 0
    let count = $state(props.initialCount);
    let doubled = $derived(count * 2);
</script>

<button on:click={() => count++}> 
    Count: {count}
</button>

<span> doubled is {doubled}</span>