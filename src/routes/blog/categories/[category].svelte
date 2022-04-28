<script context="module">
	export const load = async ({ params, fetch }) => {
		const currentCategory = params.category;
		const response = await fetch('/api/posts.json');
		const posts = await response.json();

		const matchingPosts = posts.filter((post) => post.meta.categories.includes(currentCategory));

		return {
			props: {
				posts: matchingPosts
			}
		};
	};
</script>

<script>
	export let posts;
</script>

<div class="container">
	<ul>
		{#each posts as post}
			<li>
				<h1>
					<a href={post.path}>
						{post.meta.title}
					</a>
				</h1>
				<div class="datecategoriescontainer">
					{post.meta.date}
					{#each post.meta.categories as category}
						<div class="categorycontainer">
							#{category}
						</div>
					{/each}
				</div>
				<p>
					<a href={post.path}>
						<!-- Need to make a function to calculate snippets of the blog -->
						{post.meta.snippet}
					</a>
				</p>
			</li>
		{/each}
	</ul>
</div>

<style>
	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	ul {
		list-style: none;
		padding-left: 0;
		/* width: 100%; */
		margin: 0mm;
	}
	li {
		/* border: 1px solid #dbd6d6; */
		padding: 1rem;
	}

	h1 {
		margin: 0.15rem 0rem;
	}
	.datecategoriescontainer {
		display: flex;
		align-items: center;
		gap: 1rem;
		margin: 0;
		margin-left: 0.4rem;
		padding: 0;
	}

	.categorycontainer {
		color: #fe7b43;
		font-weight: 600;
		border: 1px solid #fe7b43;
		border-radius: 0.5rem;
		padding: 0.1rem;
	}
	p {
		margin: 0.5rem;
		color: black;
	}

	a {
		text-decoration: none;
		color: black;
	}
</style>
