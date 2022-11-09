<script>
	export let title;
	export let date;
	export let categories;
</script>

<div class="post-container">
	<a class="back-button" href="/">Go Back</a>
	<h1>{title}</h1>
	{#if categories.length}
		<div class="categoriescontainer">
			<p class="date">{date}</p>
			{#each categories as category}
				<div class="categorycontainer">
					<a href="/blog-posts/categories/{category}">
						#{category}
					</a>
				</div>
			{/each}
		</div>
	{/if}
	<slot />
</div>

<style>
	/* Styles are organized from top of html to bottom */
	.post-container {
		margin: 1rem;
		margin-top: 5rem;
		margin-bottom: 3rem;
		padding: 2rem;
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
	.categorycontainer:hover {
		color: #fe7b43;
		background-color: #fe7b43;
	}

	.categorycontainer a:hover {
		color: #e7e7e7;
	}
	.categoriescontainer > p {
		margin: 0;
	}

	/* Mobile styling */
	@media screen and (max-width: 768px) {
		.post-container {
			margin: 0;
			padding: 1rem;
		}
	}

	/* styling for really big screens */
	@media screen and (min-width: 1660px) {
		.post-container {
			padding: 0 20%;
		}
	}
</style>
