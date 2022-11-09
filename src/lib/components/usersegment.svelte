<script>
	import creator from '$lib/logos/icons/creator.svg';
	import user from '$lib/logos/icons/user.svg';
	import handshake1 from '$lib/logos/icons/hand-shake-1.svg';
</script>

<div class="container my-6">
	<div class="content">
		<div class="feature-text">
			<p>Customer Segments</p>
			<h1>What type of customer are you?</h1>
			<h5 class="thirdtext mt-6">
				Our platform creates value for everybody, from viewer to data scientist.
			</h5>
		</div>
	</div>
	<div class="grid-container">
		<div class="viwer-segment">
			<div class="columns">
				<img
					class="column is-one-quarter is-one-fifth-mobile graphic smaller"
					src={user}
					alt="placholder"
				/>
				<div class="column content">
					<h4>User</h4>
					<ul>
						<li>No ads! You pay for content for as low as a fraction of a cent.</li>
						<li>Have nuanced converstions with Venn UI.</li>
						<li>Own and sell your data for a profit!</li>
						<li>You have the power! Vote, comment, tag and censor all content.</li>
					</ul>
				</div>
			</div>
		</div>

		<div class="creator-segment">
			<div class="columns">
				<img
					class="column is-one-quarter is-one-fifth-mobile graphic"
					src={creator}
					alt="placholder"
				/>
				<div class="column content">
					<h4>Creator</h4>
					<ul>
						<li>Get paid for your content! Finally focus soley on value instead of sponsors</li>
						<li>Understand your audience and further develop unique conent with Venn UI</li>
						<li>Own and sell your data for a profit!</li>
						<li>Respond to your audience quickly and accuratley with detailed voting.</li>
					</ul>
				</div>
			</div>
		</div>

		<div class="b2b-segment">
			<div class="columns">
				<img
					class="column is-one-quarter is-one-fifth-mobile graphic"
					src={handshake1}
					alt="placholder"
				/>
				<div class="column content">
					<h4>B2B</h4>
					<ul>
						<li>
							The four fundamental features: Microtransactions, Micropower, Venn UI and Data
							Dignity, create an incredible range of high quality user data.
						</li>
						<li>
							Buy high quality, ethical user data. Use it for content moderation on a chat app,
							language model data for your AI or data for related content algorithms.
						</li>
					</ul>
				</div>
			</div>
		</div>
	</div>
</div>

<style>
	.grid-container {
		display: grid;
		grid-template-columns: repeat(1, auto);
		row-gap: 2rem;
	}
	.graphic {
		width: 100px;
		height: auto;
	}
	/* .smaller {
		width: 70px;
		height: auto;
		padding: 12px;
	} */
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

	.content > h4 {
		color: #ff4d00;
	}
</style>
