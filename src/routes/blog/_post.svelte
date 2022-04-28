<script>
	export let title;
	export let date;
	export let snippet;
	export let categories;
</script>

<div class="post-container">
	<a class="back-button" href="/">Go Back</a>
	<h1>{title}</h1>
	{#if categories.length}
		<div class="categoriescontainer">
			<p>Published: {date}</p>
			{#each categories as category}
				<div class="categorycontainer">
					<a href="/blog/categories/{category}">
						{category}
					</a>
				</div>
			{/each}
		</div>
	{/if}
	<!-- Need to make a function to calculate snippets of the blog -->
	<p>{snippet}</p>
	<slot />
</div>

<style>
	.post-container {
		margin: 1rem;
	}

	.back-button {
		text-decoration: none;
		color: #575899;
		border: 1px solid #575899;
		border-radius: 0.5rem;
		padding: 0.1rem;
	}
	.back-button:hover {
		font-weight: 600;
		border: 2px solid #575899;
	}

	h1 {
		margin-bottom: 0.15rem;
	}

	.categoriescontainer {
		display: flex;
		gap: 1rem;
		align-items: center;
	}
	.categorycontainer {
		border: 1px solid #fe7b43;
		border-radius: 0.5rem;
		padding: 0.1rem;
	}
	.categorycontainer > a {
		font-weight: 600;
		text-decoration: none;
		color: #fe7b43;
	}
	.categoriescontainer > p {
		margin: 0;
	}
</style>
