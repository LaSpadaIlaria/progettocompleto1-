<script>

    // let props = $props();
    // con proprs andiamo ad accedere a un oggetto di js e poi lo sostituiamo sotto al posto dello 0
    let { initialCount: count = $bindable()} = $props();
    let doubled = $derived(count * 2);
</script>

<button onclick={() => count++}> 
    Count: {count}
</button>

<span> doubled is {doubled}</span>
