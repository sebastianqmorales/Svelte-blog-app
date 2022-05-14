<script>
	export let date;
	export let title;
	export let categories;
</script>

<div class="container">
	<h1>{title}</h1>
	{#if categories.length}
		<div class="categoriescontainer">
			<p class="date">Published: {date}</p>
			{#each categories as category}
				<div class="categorycontainer">
					<a href="/blog/categories/{category}">
						#{category}
					</a>
				</div>
			{/each}
		</div>
	{/if}
	<slot />
</div>

<style>
	.container {
		padding: 3rem;
	}

	h1 {
		margin-bottom: 0.15rem;
	}

	.categoriescontainer {
		display: flex;
		gap: 1rem;
		align-items: center;
		margin-bottom: 2rem;
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

	/* Mobile styling */
	@media screen and (max-width: 768px) {
		.container {
			margin: 0;
			padding: 1rem;
		}
	}
</style>
