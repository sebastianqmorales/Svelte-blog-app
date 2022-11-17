<script>
	import adIcon from '$lib/logos/icons/online-advertising.svg';
	import { fade } from 'svelte/transition';

	let visible = false;

	import comment from '$lib/logos/gifs/comment.svg';
</script>

<div class="container my-6">
	<div class="content mb-5">
		<div class="feature-text">
			<p>What is Cuatex?</p>
			<h1>Cuatex is a content marketplace.</h1>
			<h5 class="thirdtext mt-6">
				Our platform is run by the users and our economic model encourages valuable, reasonable and
				transparent creator content.
			</h5>
		</div>
	</div>

	<div class="is-flex is-flex-direction-column ">
		<div class="content mb-6">
			<h4 class="venn-text">The solution starts with the business model.</h4>
			<p class="text-align">
				The use of the advertisement business model creates apps that censor senstive topics, sells
				all your data and tries to be as addicting as possible.
			</p>
		</div>
		<div class="ad-container">
			<img src={adIcon} alt="graphic" class="ad-graphic" />
			<div class="content">
				<p>
					Our model relies on Microtransactions, transactions as low as a fraction of a cent to
					content creators. This model removes the needs for ads, which in turn creates a more user
					friendly and user moderated platform.
				</p>
			</div>
		</div>
	</div>
</div>
<div class="block" />
<div
	class="container my-6"
	on:mouseenter={() => {
		visible = true;
	}}
>
	<div class="columns is-vcentered my-6">
		<div class="column content is-three-fifths">
			<h4>Vertical content has deeper implications.</h4>
			<p>
				Ever wonder why a comment section lacks diversity of thought? The vertical structure of the
				most popular apps encourage echo chambers and attention seekers.
			</p>
		</div>
		<div class="column vertanimation">
			{#if visible}
				{#each { length: 3 } as _, i}
					<img
						in:fade={{ duration: 2000, delay: 300 * i }}
						src={comment}
						alt="gif"
						class="vertanimation my-4"
					/>
				{/each}
			{/if}
		</div>
	</div>
	<div class="is-flex is-flex-direction-column ">
		<div class="content mb-6">
			<h4 class="venn-text">Our unique Venn UI encourages nuanced converstions.</h4>
			<p class="text-align">
				By replacing the vertical structure of comment and content feeds we get more diverse and
				intersting perspectives. This 2-dimensional design, what we call "Venn UI", creates a more
				transparent and balanced place for people to share their thoughts.
			</p>
		</div>
		<div class="venn-graphic">
			{#if visible}
				{#each { length: 9 } as _, i}
					<img in:fade={{ duration: 2000, delay: 300 * i }} src={comment} alt="gif" class="gif" />
				{/each}
			{/if}
		</div>
	</div>
</div>

<style>
	.ad-container {
		display: grid;
		grid-template-columns: repeat(2, auto);
		column-gap: 3rem;
		align-items: center;
	}

	.ad-graphic {
		transform: scale(0.7);
	}

	.block {
		margin-top: 6rem;
	}

	.vertanimation {
		display: grid;
		grid-template-columns: repeat(1, auto);
	}

	.venn-graphic {
		display: grid;
		grid-template-columns: repeat(3, auto);
		row-gap: 2rem;
		column-gap: 1.25rem;
	}
	.feature-text {
		text-align: center;
		margin-bottom: 7rem;
	}
	.feature-text > h1 {
		color: #ff4d00;
	}
	.thirdtext {
		padding-left: 20%;
		padding-right: 20%;
		line-height: 2rem;
		/* color: #fe7b43; */
		font-weight: 500;
	}

	.venn-text {
		text-align: center;
	}
	.text-align {
		text-align: center;
	}
</style>
