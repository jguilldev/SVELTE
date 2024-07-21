<!-- La estructura  de componentes tiene 3 partes el script el css y la -->


<script>// Aqui va la logica

let algunTexto = "Este es mi primer texto en svelte" //Se crea el contenido en este caso un string

</script>

<style>  
/* Aqui van los estilos, colores tipo de letra etc, con css */
p{
    display: inline-block;
    color: red;
    font-size:80%;
    width: 30%;
    height: 30%;
}

</style>
<!-- Este div es donde se traen los componentes o el contenido a mostrar -->
<div class="contenido"> <!-- Se recomienda poner en un div el contenido propio del componente -->
<p>
    {algunTexto}
</p>

</div>