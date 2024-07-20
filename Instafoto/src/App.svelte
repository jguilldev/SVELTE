<script> // Aqui debo traer o importar
	export let name;
	export let LastName;
	// let componente;  se declara asi para trer un nuevo componente 
</script>

<main>  <!-- en main van los componentes que se van a visualizar es decir aqui traemos los componentes creados -->
	<h1>Hello {name} {LastName}!</h1>

	
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>