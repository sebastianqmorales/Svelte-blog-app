<script>
	import Map from '$lib/logos/map-project-img.png';
</script>

<div class="container">
	<h1>Who is Sebastian?</h1>
	<slot />
	<h1>Projects</h1>
	<img src={Map} alt="map project" class="portimage" />
	<a class="btn" href="https://maptyworkoutapp.netlify.app/">Live Site</a>
	<h1>Contact</h1>
</div>

<style>
	.container {
		padding: 3rem;
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.portimage {
		aspect-ratio: 18/ 8;
		height: 20rem;
	}

	.btn {
		color: #fff;
		font-family: inherit;
		text-decoration: none;
		font-size: 20px;
		font-weight: 900;
		background-color: #000;
		border: 1px solid #fe7b43;
		padding: 20px 20px;
		border-radius: 3px;
		line-height: 0.428571;
		position: absolute;
		z-index: 1;
		letter-spacing: -0.2px;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
	}
</style>
