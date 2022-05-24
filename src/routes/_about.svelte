<div class="container">
	<a class="back-button" href="/">Go Back</a>
	<h1>About Cuatex</h1>
	<slot />
</div>

<style>
	.container {
		margin: 1rem;
		margin-top: 3rem;
		margin-bottom: 3rem;
		padding: 2rem;
	}

	.back-button {
		text-decoration: none;
		color: #575899;
		border: 1px solid #575899;
		border-radius: 0.5rem;
		padding: 0.1rem;
	}
	.back-button:hover {
		font-weight: 600;
		border: 2px solid #575899;
	}

	/* styling for really big screens */
	@media screen and (min-width: 1660px) {
		.container {
			padding: 0 20%;
		}
	}
</style>
