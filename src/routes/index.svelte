<script>
	import '$lib/styles/style.scss';
	import Cta from '$lib/components/emailcta.svelte';
	import Card from '$lib/components/card.svelte';
	import LeftCard from '$lib/components/leftcard.svelte';
	import Header from '$lib/components/header.svelte';
</script>

<Header />
<div class="container">
	<section class="section gradient mt-5">
		<div class="content">
			<div class="feature-text">
				<p>Top Features</p>
				<h1>A people first expeirence</h1>
				<h5 class="thirdtext mt-6">
					Make sure your perspective is heard with Linked Venn UI. Earn money from users directly
					paying you per view. Own your data and earn money by selling it!
				</h5>
			</div>
		</div>
		<Card />
	</section>
	<section class="section">
		<LeftCard />
	</section>
	<section class="section flipped-gradient mb-5">
		<Card />
	</section>
	<Cta />
</div>

<style>
	/* Alot of the style is coming from the html tags applying styles from 
	a Bulma CDN that islinked in the Styles.scss file
	*/
	.feature-text {
		text-align: center;
		margin-bottom: 7rem;
	}
	.feature-text > p {
		color: #2a6397;
	}
	.feature-text > h1 {
		color: #2d4628;
	}
	.thirdtext {
		padding-left: 20%;
		padding-right: 20%;
		line-height: 2rem;
		/* color: #fe7b43; */
		color: #405f3af6;
		font-weight: 500;
	}

	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		row-gap: 40px;
	}
	.gradient {
		background: linear-gradient(180deg, rgba(255, 76, 0, 0.08) 0%, rgba(255, 255, 255, 0) 100%);
		width: 100%;
		padding-top: 50px;
	}

	.flipped-gradient {
		background: linear-gradient(180deg, rgba(217, 217, 217, 0) 0%, rgba(254, 123, 67, 0.15) 100%);
	}

	:root {
		--blur: 2.52px;
		--spread: -1.8px;
		--horiz: -1.43754px;
		--vert: 1.08327px;
	}

	.card {
		box-shadow: calc(clamp(0px, var(--horiz), 2px)) calc(clamp(0px, var(--vert), 2px)) 2px
				calc(var(--spread)) rgba(0, 0, 0, 0.233),
			calc(2 * var(--horiz)) calc(2 * var(--vert)) calc(var(--blur)) calc(var(--spread))
				rgba(0, 0, 0, 0.2),
			calc(3 * var(--horiz)) calc(3 * var(--vert)) calc(var(--blur)) calc(var(--spread))
				rgba(0, 0, 0, 0.123),
			calc(5 * var(--horiz)) calc(5 * var(--vert)) calc(var(--blur)) calc(var(--spread))
				rgba(0, 0, 0, 0.076),
			calc(8 * var(--horiz)) calc(8 * var(--vert)) calc(var(--blur)) calc(var(--spread))
				rgba(0, 0, 0, 0.047),
			calc(13 * var(--horiz)) calc(13 * var(--vert)) calc(var(--blur)) calc(var(--spread))
				rgba(0, 0, 0, 0.028);
		border: 1px solid rgba(0, 0, 0, 0.068);

		height: 300px;
		width: 200px;
	}
</style>
