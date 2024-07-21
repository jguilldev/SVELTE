<script>
 export let mensaje = "Este es el mensaje de condicional mostrandose"
 export let mensaje2 = "Este es el otro mensaje concdicional"

 let estado = true

 function cambiar(){
    estado = !estado
 }

</script>

<style>

</style>

<div>
    {#if estado == true}
    <p>{mensaje}</p>
    {:else}
    <p>{mensaje2}</p>
    {/if}

    <button on:click={cambiar}>CAMBIA MENSAJE (IF)</button>
</div>