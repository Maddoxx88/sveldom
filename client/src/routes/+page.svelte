<script>
	import Games from '$lib/components/games-list.svelte';
	import Landing from '$lib/components/landing.svelte';
	import Header from '$lib/header.svelte';
	import '../app.css';
</script>

<Header />
<Landing />
<Games />

<slot />
