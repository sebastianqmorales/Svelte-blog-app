<script>
	import icon1 from '$lib/logos/icons/dollar-bills-stack.svg';
	import icon2 from '$lib/logos/icons/binary.svg';
	import icon3 from '$lib/logos/icons/vote.svg';
	import icon4 from '$lib/logos/icons/venn-diagram.svg';
</script>

<div class="container">
	<div class="content">
		<div class="feature-text">
			<p>Fundamental Features</p>
			<h1>A people-first experience.</h1>
			<h5 class="thirdtext mt-6">
				Make your perspective heard with our Venn design. Earn money from users directly paying you.
				Own and monetize your own data!
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
							No ads! You pay for content and can sell it at whatever price you want, starting at 1
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
							We don't need your data! Own your data and opt into our Data Union program to sell it!
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
						<p>
							No AI. We let you tag and censor inappropriate content&mdash;and earn money from it!
						</p>
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
							No echo chambers. Our innovative Venn design encourages easy sharing of unique
							perspectives.
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
		transform: scale(0.65);
	}

	.content > h4 {
		color: #ff4d00;
	}
</style>
