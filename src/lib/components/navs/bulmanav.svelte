<script>
	import logo from '$lib/logos/CuatexFullLogo.svg';
	let active = '';
	function handle() {
		active = !active;
	}
</script>

<!-- svelte-ignore a11y-no-redundant-roles -->
<nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
	<div class="navbar-brand">
		<a class="logo" href="/">
			<img src={logo} alt="Cuatex Logo" class="ml-5" />
		</a>

		<!-- svelte-ignore a11y-missing-attribute -->
		<a
			on:click={handle}
			role="button"
			class="navbar-burger {active ? 'is-active' : ''}"
			aria-label="menu"
			aria-expanded="false"
			data-target="navbarBasicExample"
		>
			<span aria-hidden="true" />
			<span aria-hidden="true" />
			<span aria-hidden="true" />
		</a>
	</div>

	<div id="navbarBasicExample" class="navbar-menu {active ? 'is-active' : ''}">
		<div class="navbar-end">
			<div class="navbar-item" on:click={handle}>
				<a class="link navbar-item mr-5" sveltekit:prefetch href="/about">About</a>
				<a class="link navbar-item mr-5" sveltekit:prefetch href="/blog">Blog</a>
			</div>
		</div>
	</div>
</nav>

<style>
	.link {
		color: #ff4d00;
		font-weight: 500;
	}
</style>
