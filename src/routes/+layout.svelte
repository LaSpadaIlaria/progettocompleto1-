<script>
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}


<!-- tuttto quello che viene messo qui lo ritroviamo in tutte le pagine -->

<footer>
	<p>Copyright 2024</p>
</footer>

<!-- svelte ha la capacità di non far mandare in cnflitto il css, quindi trasofrma le cose in container. restringe il campo di azione al css al file -->


<!-- 1- adesso vogliamo avere lo stile globale. prendo e sposto lo stile in page a layout e poi aggiungo :global e nelle parentesi la cosa a cui è rivolto-->

 <style>
    :global(p)  {
        color: rgb(150, 0, 143);
    }
</style>
