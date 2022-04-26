<script>
	export let title;
	export let date;
	export let snippet;
</script>

<h1>{title}</h1>
<p>Published: {date}</p>
<p>{snippet}</p>

<slot />
