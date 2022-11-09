<div class="container">
	<a class="back-button mb-6" href="/">Go Back</a>
	<h1>About Cuatex</h1>
	<slot />
</div>

<style>
	.container {
		margin-left: 4rem;
		margin-right: 4rem;
		margin-top: 8rem;
		margin-bottom: 3rem;
		padding: 2rem;
	}

	.back-button:hover {
		font-weight: 600;
		border: 2px solid #575899;
	}
	.back-button {
		text-decoration: none;
		color: #575899;
		border: 1px solid #575899;
		border-radius: 0.5rem;
		padding: 0.1rem;
		margin-bottom: 3rem;
	}

	/* Mobile styling */
	@media screen and (max-width: 768px) {
		.container {
			margin-top: 8rem;
			margin-bottom: 3rem;
			margin-left: 1.5rem;
			margin-right: 1.5rem;
			padding: 1rem;
		}
	}
	/* styling for really big screens */
	@media screen and (min-width: 1660px) {
		.container {
			padding: 0 20%;
		}
	}
</style>
