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