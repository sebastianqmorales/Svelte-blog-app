<section class="section is-medium">
	<div class="container is-max-desktop">
		<div class="heading-text mt-6">Share your perspective.</div>
		<div class="heading-description">
			Cuatex creates economic incentives for sharing unique, valuable and thought-provoking content.
		</div>
		<div class="read-more my-4">
			Keep reading to understand how we provide a space for critical thinking without censorship,
			algorithms or ads.
		</div>
		<div class="my-5">
			<form
				class="is-flex form1 field"
				name="top-email"
				method="POST"
				netlify-honeypot="nbot-field"
				data-netlify="true"
			>
				<input type="hidden" name="form-name" value="top-email" />
				<input
					name="email"
					id="email"
					class="input"
					type="text"
					required
					placeholder="example@gmail.com"
				/>
				<p class="help" />
				<input type="submit" class="button " value="Notify me of launch!" />
			</form>
		</div>
	</div>
</section>

<style>
	.section {
		background-color: #fe7b43;
		width: 100%;
		background-image: url('$lib/logos/Header-Background.svg');
		background-repeat: repeat-y;
		background-position: right;
	}

	.form1 {
		margin-top: 0px;
		margin-bottom: 0px;
	}
	.input {
		border-top-right-radius: 0px;
		border-bottom-right-radius: 0px;
		border: 0px;
		font-size: calc(11px + 0.390625vw);
	}
	.button {
		margin: 0px !important;
		border-bottom-left-radius: 0px;
		border-top-left-radius: 0px;
		border: 0px;
		background-color: #ff4d00;
		font-weight: 700;
		font-size: calc(11px + 0.390625vw);
	}
	.heading-text {
		/* font-size: 2rem; */
		font-size: calc(2rem + 0.90625vw);
		font-weight: 700;
		line-height: 2.5rem;
		padding-top: 30px;
		padding-bottom: 20px;
	}

	.heading-description,
	.read-more {
		font-size: calc(15px + 0.390625vw);
		font-weight: 500;
	}
</style>
