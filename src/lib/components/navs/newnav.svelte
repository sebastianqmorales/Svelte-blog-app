<script>
	import { page } from '$app/stores';
	import logo from '$lib/logos/CuatexFullLogo.svg';
</script>

<nav class="navbar is-fixed-top is-flex is-flex-direction-row is-justify-content-space-between">
	<a class="logo" href="/">
		<img src={logo} alt="Cuatex Logo" />
	</a>

	<div class="right is-flex is-align-content-center is-align-self-center">
		<a class="link" sveltekit:prefetch href="/about">About</a>
		<a class="link" sveltekit:prefetch href="/blog">Blog</a>
	</div>
</nav>

<style>
	/* Alot of the style is coming from the html tags applying styles from a Bulma CDN that is linked in the Styles.scss file*/
	.logo {
		padding-left: 4rem;
	}
	.logo img {
		display: block;
	}
	.link {
		text-decoration: none;
		font-weight: 600;
		color: #fe7b43;
		/* padding: 0.35rem; */
	}
	.right {
		column-gap: 3rem;
		padding-right: 4rem;
	}
</style>
