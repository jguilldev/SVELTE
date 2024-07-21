<script>
    export let texto = "Aun no hay valor de prop"; // Se le dio valor por defecto a texto = "Aun no hay valor"
    // El prop (texto) es algo vacío en este caso text que se puede importar a la aplicación principal 
    // App.svelte, y allí darle el valor, sin embargo es necesario llamarlo en este componente desde
    // el dispatchEvent, que está más abajo
</script>

<div class="texto">
    <p>
        {texto}<!-- Aquí llamamos el prop dentro del div, pero su valor se le da en App.svelte -->
    </p>
</div>
