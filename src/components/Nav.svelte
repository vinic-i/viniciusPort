<script>
	let y = 0;
	let open = false;
</script>

<svelte:window bind:scrollY={y} />

<!-- Navigation-->
<nav class="navbar navbar-expand-lg fixed-top navbar-dark bgNav-dark">
	<a class="navbar-brand" on:click={() => (open = false)} href="#page-top">
		Home
	</a>

	<button
		class=" navbar-toggler navbar-toggler-center"
		style="color:white"
		type="button"
		on:click={() => (open = !open)}
		aria-expanded={open}>
		<i class="fas fa-bars" />
	</button>
	<div
		class=" collapse navbar-collapse {open ? 'show' : ''}"
		id="navbarResponsive"
	>
		<ul class="navbar-nav ml-auto text-center">
			<li class="nav-item">
				<a
					class="nav-link"
					on:click={() => (open = false)}
					href="#about">Sobre</a
				>
			</li>

			<li class="nav-item">
				<a
					class=" nav-link"
					on:click={() => (open = false)}
					href="#projects">Projetos</a
				>
			</li>
			<li class="nav-item">
				<a
					class="white nav-link"
					on:click={() => (open = false)}
					href="#features">Ferramentas</a
				>
			</li>
			<li class="nav-item">
				<a
					class=" nav-link"
					on:click={() => (open = false)}
					href="#signup">Contatos</a
				>
			</li>
		</ul>
	</div>
</nav>

<style>
	.nav-item {
		background-color: black;
	}
	.nav-item a{
		color: rgb(189, 184, 184)
	}
	.navbar a{
		color: rgb(189, 184, 184)
	}
	.nav-item:hover a {
		color:white !important;
	}
	.navbar-brand:hover  {
		color:white !important;
	}
	ul {
		background-color: black;
	}
	.white {
		color: white;
	}
</style>
