<!-- <script>
	import logo from '$lib/logos/CuatexFullLogo.svg';
</script> -->

<div class="container is-max-desktop">
	<div class="cta-message">
		Be the first to create an account and claim a user name! Sign up to be notified of our launch.
	</div>
	<form class="field mb-0" name="username" method="POST" data-netlify="true">
		<!-- svelte-ignore a11y-label-has-associated-control -->
		<label class="label mb-0 mt-1">Email</label>
		<div class="control">
			<input class="input" type="email" placeholder="example@gmail.com" />
		</div>
		<p class="help " />
	</form>
	<div class="button mt-0">Submit</div>
	<div class="email-disclaimer mt-4">
		By submitting this form you consent to us emailing you occasionally about our products and
		services. You can unsubscribe from emails at any time, and we will never pass your email to
		third parties.
	</div>
</div>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400&display=swap');
	* {
		font-family: 'Roboto', sans-serif;
	}
	.cta-message {
		font-family: 'Roboto', sans-serif;
		font-weight: bold;
		color: black;
		text-align: center;
		font-size: larger;
	}
	.container {
		display: flex;
		flex-direction: column;
		background-color: #fe7b43;
		padding-left: 100px;
		padding-right: 100px;
		padding-top: 10px;
		padding-bottom: 10px;
		border: 1px solid #fe7b43;
		border-radius: 10px;
	}
	.button {
		background-color: #ff4d00;
		font-weight: bolder;
		letter-spacing: 1px;
		border: 0px;
	}
	.button:hover {
		transform: scale(1.05);
	}

	@media screen and (max-width: 768px) {
		.container {
			padding-left: 10px;
			padding-right: 10px;
		}
	}
</style>
