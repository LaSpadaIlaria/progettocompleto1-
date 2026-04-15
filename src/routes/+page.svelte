<script>
    let count = $state(0);
    let doubled = $derived(count * 2);
</script>
<!-- 2-abbiamo fatto questa cosa di creare una variabile e di far partire il contatore da 0. allora creo un button nel 3-->
 <!-- 4-faccio anche la variabile doubled per il bottone che raddoppia -->

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the documentation</p>

<!-- 3-creiamo un bottone in cui gli diciamo che al click deve eseguire questa funzione in cui fa +1. viene preso il valore di count da sopra e count viene sostituito da qui -->
<button on:click={() => count++}>
    Count: {count}
</button>



<!-- 5-creiamo un bottone in cui gli diciamo che al click deve eseguire questa funzione in cui raddoppia il valore di count. viene preso il valore di doubled da sopra e doubled viene sostituito da qui -->
<span> doubled is {doubled}</span>

<!-- questa è la struttura classica di un file svelte, abbiamo script quindi js per primo, poi abbiamo html e infine css -->