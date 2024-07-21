<!-- La propagacion es tener un objeto con elementos en el APP.svelte,
  y poder pasarselo a otros elementos  -->

<script> 
    // se declaran los tres tipos dentro del objeto en el script de app.svelte
    export let name 
    export let lastName 
    export let age 
</script>

<div class="Propagacion">
    <p>
        {name} {lastName} {age} 
        <!-- En la linea anteriorse declararon los tipos dentro del objeto en el script de app.svelte -->
    </p>
</div>