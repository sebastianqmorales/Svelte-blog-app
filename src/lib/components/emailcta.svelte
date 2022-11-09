<div class="container is-max-desktop my-6">
	<div class="cta-title mb-4">
		Help us end media manipulation. Sign up to be notified of our launch.
	</div>
	<form
		class="is-flex is-flex-direction-column field mb-0"
		name="email"
		method="POST"
		netlify-honeypot="bot-field"
		data-netlify="true"
	>
		<input type="hidden" name="form-name" value="email" />
		<input class="input" type="email" placeholder="example@gmail.com" />
		<p class="help " />
		<input type="submit" class="button mt-1" value="Submit" />
	</form>
	<div class="email-disclaimer mt-5">
		By submitting this form you consent to us emailing you occasionally about our products and
		services. You can unsubscribe from emails at any time, and we will never pass your email to
		third parties.
	</div>
</div>

<style>
	* {
		font-family: 'Poppins', sans-serif;
	}
	.cta-title {
		font-weight: bold;
		color: black;
		text-align: center;
		font-size: 1.5rem;
	}
	.container {
		display: flex;
		flex-direction: column;
		background-color: #fe7b43;
		padding-left: 140px;
		padding-right: 140px;
		padding-top: 10px;
		padding-bottom: 10px;
		border: 1px solid #fe7b43;
		border-radius: 10px;
		background-image: url('$lib/logos/Container-Background.svg');
	}
	.button {
		background-color: #ff4d00;
		font-weight: 700;
		letter-spacing: 1px;
		border: 0px;
		font-size: 1.2rem;
	}
	.button:hover {
		transform: scale(1.05);
	}

	.email-disclaimer {
		font-weight: 400;
		text-align: center;
		font-size: 0.85rem;
	}

	@media screen and (max-width: 768px) {
		.container {
			padding-left: 10px;
			padding-right: 10px;
		}
	}
</style>
