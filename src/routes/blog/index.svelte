<script context="module">
	export const load = async ({ fetch }) => {
		const posts = await fetch('/api/posts.json');
		const allPosts = await posts.json();

		return {
			props: {
				posts: allPosts
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
				<p>
					Published {post.meta.date}
				</p>
				<p>
					<a href={post.path}>
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
	}
	li:nth-child(2) {
		margin: 1.5rem 0rem;
	}

	h1 {
		margin: 0.15rem;
	}

	p {
		margin: 0.5rem;
	}

	a {
		text-decoration: none;
		color: black;
	}
</style>
