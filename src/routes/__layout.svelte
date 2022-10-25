<script>
	import Nav from '../lib/components/nav.svelte';
	import Nav2 from '$lib/components/newnav.svelte';
	import Nav3 from '$lib/components/bulmanav.svelte';
	import '$lib/styles/style.scss';
</script>

<main>
	<Nav3 />
	<slot />
</main>
