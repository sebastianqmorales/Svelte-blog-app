<script>
	import Nav from '../lib/components/navs/nav.svelte';
	import Nav2 from '$lib/components/navs/newnav.svelte';
	import Nav3 from '$lib/components/navs/bulmanav.svelte';
	import '$lib/styles/style.scss';
</script>

<main>
	<Nav3 />
	<slot />
</main>
