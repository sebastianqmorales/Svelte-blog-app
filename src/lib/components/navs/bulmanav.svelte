<script>
	import logo from '$lib/logos/CuatexFullLogo.svg';
</script>

<nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
	<div class="navbar-brand">
		<a class="logo" href="/">
			<img src={logo} alt="Cuatex Logo" />
		</a>

		<a
			role="button"
			class="navbar-burger"
			aria-label="menu"
			aria-expanded="false"
			data-target="navbarBasicExample"
		>
			<span aria-hidden="true" />
			<span aria-hidden="true" />
			<span aria-hidden="true" />
		</a>
	</div>

	<div id="navbarBasicExample" class="navbar-menu">
		<div class="navbar-end">
			<div class="navbar-item">
				<a class="link" sveltekit:prefetch href="/about">About</a>
				<a class="link" sveltekit:prefetch href="/blog">Blog</a>
			</div>
		</div>
	</div>
</nav>
