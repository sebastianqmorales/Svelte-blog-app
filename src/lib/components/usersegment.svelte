<script>
	import placeholder from '$lib/logos/placeholder.png';
	import icon4 from '$lib/logos/icons/venn-diagram.svg';
	import creator from '$lib/logos/icons/creator.svg';
	import user from '$lib/logos/icons/user.svg';
	import handshake1 from '$lib/logos/icons/hand-shake-1.svg';
	import handshake2 from '$lib/logos/icons/hand-shake-2.svg';
</script>

<div class="container">
	<div class="content">
		<div class="feature-text">
			<p>Customer Segments</p>
			<h1>What type of customer are you?</h1>
			<h5 class="thirdtext mt-6">
				Our platform creates value for everybody, from viewer to data scientist.
			</h5>
		</div>
	</div>
	<div class="is-flex is-flex-direction-column">
		<div class="is-flex">
			<div class="viwer-segment">
				<div class="columns">
					<img
						class="coloumn is-one-quarter is-one-fifth-mobile graphic smaller"
						src={user}
						alt="placholder"
					/>
					<div class="coloumn content">
						<h4>User</h4>
						<p>
							No ads, earn money from voting, commenting and more, always have the ability to vote
							and comment, Venn UI allows you to share your unique perspective
						</p>
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
						<p>
							No ads, earn money from voting, commenting and more, always have the ability to vote
							and comment, Venn UI allows you to share your unique perspective
						</p>
					</div>
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
					<p>
						No ads, earn money from voting, commenting and more, always have the ability to vote and
						comment, Venn UI allows you to share your unique perspective
					</p>
				</div>
			</div>
		</div>
	</div>
</div>

<style>
	.graphic {
		width: 100px;
		height: auto;
	}
	.smaller {
		width: 60px;
		height: auto;
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

	.content > h4 {
		color: #ff4d00;
	}
</style>
