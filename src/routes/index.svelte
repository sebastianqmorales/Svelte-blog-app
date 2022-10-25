<script>
	import '$lib/styles/style.scss';
	import Cta from '$lib/components/emailcta.svelte';
	import Card from '$lib/components/card.svelte';
	import Header from '$lib/components/header.svelte';
</script>

<Header />
<div class="container">
	<section class="section gradient mt-5">
		<div class="text mt-5 mb-5">
			What is Cuatex? To understand Cuatex you need to understand the current revenue models of the
			internet. The most popular platforms on the internet use an advertisement model, to give the
			user free access to the internet and give the creator some chance of making money through ad
			watch.
		</div>
		<Card />
	</section>

	<div class="gradient-flipped">
		gradient container
		<div class="card">card 3</div>
		<div class="statment">statment 3</div>
	</div>
	<div class="email-cta">
		<div class="top">top description</div>
		<div class="capture">input part</div>
		<div class="button">button to approve of input</div>
	</div>
	<div class="read">read our blog section</div>
	<Cta />
</div>

<style>
	/* Alot of the style is coming from the html tags applying styles from a Bulma CDN that is linked in the Styles.scss file*/
	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		row-gap: 10px;
	}
	.gradient {
		background: linear-gradient(180deg, rgba(255, 76, 0, 0.08) 0%, rgba(255, 255, 255, 0) 100%);
		width: 100%;
		padding-top: 50px;
	}
	.text {
		font-weight: 500;
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
