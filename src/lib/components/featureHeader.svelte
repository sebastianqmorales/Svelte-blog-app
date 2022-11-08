<script>
	import placeholder from '$lib/logos/placeholder.png';
	import icon1 from '$lib/logos/icons/dollar-bills-stack.svg';
	import icon2 from '$lib/logos/icons/binary.svg';
	import icon3 from '$lib/logos/icons/vote.svg';
	import icon4 from '$lib/logos/icons/venn-diagram.svg';
</script>

<div class="container">
	<div class="content">
		<div class="feature-text">
			<p>Top Features</p>
			<h1>A people first expeirence</h1>
			<h5 class="thirdtext mt-6">
				Make sure your perspective is heard with our Venn design. Earn money from users directly
				paying you. Own your data and earn money by selling it!
			</h5>
		</div>
	</div>
	<div class="columns">
		<div class="column">
			<div class="columns">
				<div class="column is-one-quarter is-one-fifth-mobile ">
					<img class="graphic" src={icon1} alt="icon" />
				</div>
				<div class="column">
					<div class="content">
						<h4>Microtransactions</h4>
						<p>
							No ads, you pay for content and can sell it at whatever price you want, starting at 1
							cent per view!
						</p>
					</div>
				</div>
			</div>
		</div>
		<div class="column">
			<div class="columns">
				<div class="column is-one-quarter is-one-fifth-mobile">
					<img class="graphic" src={icon2} alt="icon" />
				</div>
				<div class="column">
					<div class="content">
						<h4>Data Dignity</h4>
						<p>
							Since you pay for content, we don't need your data! Own your data and opt into our
							Data Union program to sell it!
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>
	<div class="columns">
		<div class="column">
			<div class="columns">
				<div class="column is-one-quarter is-one-fifth-mobile">
					<img class="graphic" src={icon3} alt="icon" />
				</div>
				<div class="column">
					<div class="content">
						<h4>Micropower</h4>
						<p>No Ai needed, we let you censor inappropriate content and earn money from it!</p>
					</div>
				</div>
			</div>
		</div>
		<div class="column">
			<div class="columns">
				<div class="column is-one-quarter is-one-fifth-mobile">
					<img class="graphic" src={icon4} alt="icon" />
				</div>
				<div class="column">
					<div class="content">
						<h4>Venn UI</h4>
						<p>
							No echo chambers, our innovative Venn design encourages sharing unique perspectives
							while being easy to use.
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>

<style>
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
	.graphic {
		transform: scale(0.5);
	}

	.content > h4 {
		color: #ff4d00;
	}
</style>
