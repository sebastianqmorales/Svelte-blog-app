<script>
	import logo from '$lib/logos/CuatexFullLogo.svg';
</script>

<div class="container">
	<div class="logo"><img src={logo} alt="Cuatex Logo" /></div>
	<div class="cta-message">
		Be the first to create an account and claim a user name! Sign up to be notified of our launch.
	</div>
	<form name="cta" method="post" data-netlify="true" class="cta-input">
		<label>Reserve your username <input type="name" name="username" /> </label>
		<label>Email <input type="email" name="email" /> </label>
	</form>
	<div class="email-submission">this will be the submission button</div>
	<div class="email-disclaimer">
		By submitting this form you consent to us emailing you occasionally about our products and
		services. You can unsubscribe from emails at any time, and we will never pass your email to
		third parties.
	</div>
</div>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400&display=swap');
	/* .logo img {
		position: relative;
	} */
	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		width: 700px;
		/* margin-left: 10%;
		margin-right: 10%;
		margin-top: 0px; */
		margin-bottom: 20px;
		padding: 50px;
		border: 1px solid #fe7b43;
		border-radius: 10px;
	}

	.cta-message {
		font-family: 'Roboto', sans-serif;
		font-weight: bold;
		color: black;
		text-align: center;
	}

	.cta-input {
		display: flex;
		flex-direction: column;
		align-items: center;
		border: 1px solid black;
		background-color: #fff;
	}

	.cta-input label {
		border: 1px solid black;
	}

	.cta-input input {
		border: 0px;
	}
</style>
