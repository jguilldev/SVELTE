<script>
    // Aquí debo traer o importar
    import Nuevocomponente from "./components/Nuevocomponente.svelte"; // Importo el componente desde su ubicación
    import Props from "./components/Props.svelte";
    import Contador from "./components/contador.svelte";
    import Propagacion from "./components/Propagacion.svelte";
    import Condicionales from "./components/Condicionales.svelte";
    // export let name; Así se declara cuando no se trae el componente
    // export let LastName; Así se declara cuando no se trae el componente
    // let componente; se declara así para traer un nuevo componente 
    import Skills from "./components/Skills.svelte";

    const data = {
        name: "Guillermo",
        lastName: "Vasquez",
        age: 39,
    }

    function dark() {
        // Esta función alterna la clase dark_mode en el body
        document.body.classList.toggle('dark_mode');
    }
</script>

<main>  <!-- En main van los componentes que se van a visualizar, es decir, aquí traemos los componentes creados -->
    <!-- <Nuevocomponente/> -->
    <Contador/>
    <Props texto='Se le dio valor al prop'/> <!-- Aquí se le dio valor al prop -->
    <Props /> <!-- Aquí se debería usar el valor por defecto al prop desde el componente Props.svelte en el script -->
    <Propagacion name={data.name} lastName={data.lastName} age={data.age}/> <!-- Se declara de donde viene cada valor del objeto
    es importante usar el .data o como se haya nomrado el objeto -->

    <!-- para no usar todo:

         <Propagacion name={data.name} lastName={data.lastName}  age={data.age}/>

    es posible desestructurar data usando

        <Propagacion {..App.data}/> -->

    <button on:click={dark}>dark-mode</button> <!-- Aquí se añadió el evento on:click con la función dark -->
	<Condicionales/>

    <Skills

</main>

<style>
    main {
        text-align: center;
        padding: 1em;
        max-width: 240px;
        margin: 0 auto;
    }

    :global(body.dark_mode) {
        background-color: #1d3040;
        color: #bfc2c7;
    }

    @media (min-width: 640px) {
        main {
            max-width: none;
        }
    }
</style>
