<script>
	let y = 0;
	let open = false;
</script>

<svelte:window bind:scrollY={y} />

<!-- Navigation-->
<nav class="navbar navbar-expand-lg fixed-top navbar-dark bgNav-dark">
	<a class="navbar-brand" on:click={() => (open = false)} href="#page-top">
		Vinicius
	</a>

	<button
		class=" navbar-toggler navbar-toggler-center"
		type="button"
		on:click={() => (open = !open)}
		aria-expanded={open}>
		<i class="fas fa-bars" />
	</button>
	<div
		class=" collapse navbar-collapse {open ? 'show' : ''}"
		id="navbarResponsive"
	>
		<ul class="navbar-nav ml-auto">
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
					class=" nav-link"
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
	a:hover {
		color: var(--primary);
	}
</style>
