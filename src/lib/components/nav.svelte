<script>
	import { page } from '$app/stores';
	import logo from '$lib/logos/CuatexFullLogo.svg';
</script>

<header>
	<nav>
		<a class="logo" href="/">
			<img src={logo} alt="Cuatex Logo" />
		</a>

		<div class="right">
			<a class="about" sveltekit:prefetch href="/about">About this blog</a>
			<a class="portfolio" sveltekit:prefetch href="/featured">Featured</a>
		</div>
	</nav>
</header>
<div class="test">
	<div class="bottomNav">
		<a href="/" class="about">Home</a>
		<a href="/about" class="about">About</a>
		<a href="/featured" class="portfolio">Featured</a>
	</div>
</div>

<style>
	/* i like this nav style more than the first one */
	/* overall styles for nav */
	header {
		position: sticky;
		top: 0px;
	}
	nav {
		/* background-color: #dbd6d6; */
		background-color: #e7e7e7;
		display: flex;
		justify-content: space-between;
		padding: 0rem 2rem;
	}
	/* logo styling */
	.logo img {
		display: block;
	}
	/* styles to the right of the logo */
	.right {
		display: flex;
		align-items: center;
		column-gap: 3rem;
	}
	/* About link stlye */
	.about {
		text-decoration: none;
		font-weight: 600;
		color: #fe7b43;
		border: 1px #fe7b43 solid;
		padding: 0.35rem;
		border-radius: 35rem;
	}
	/* Portfolio button styling */
	.portfolio {
		color: #fe7b43;
		border: 1px #fe7b43 solid;
		text-decoration: none;
		padding: 0.35rem;
		border-radius: 35rem;
		border: 1px solid;
		align-self: center;
		font-weight: 600;
	}

	/* hiding bottom nav for regular use */
	.bottomNav {
		display: none;
	}
	/* bottom nav for mobile */
	@media screen and (max-width: 768px) {
		/* .test {
			position: sticky;
		} */
		.bottomNav {
			overflow: hidden;
			background-color: #e7e7e7;
			position: fixed;
			display: flex;
			justify-content: space-around;
			bottom: 0;
			width: 100%;
			padding: 0.5rem;
		}

		.bottomNav a {
			float: left;
			display: block;
			text-align: center;
			text-decoration: none;
		}
		.right {
			display: none;
		}
		nav {
			justify-content: space-evenly;
		}
	}

	/* styling for really big screens */

	@media screen and (min-width: 1660px) {
		nav {
			padding: 0 20%;
		}
	}
</style>
