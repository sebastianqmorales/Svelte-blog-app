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
