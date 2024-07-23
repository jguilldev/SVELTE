<script>
    export let count = 0; // Inicializamos el contador con un valor predeterminado de 0
    export let text = "Click me"; // Texto por defecto del botón

    function increment() {
        count += 1; // Incrementa el contador al hacer clic
    }
</script>

<!-- El botón incrementa el contador al hacer clic -->
<button on:click={increment}>
    {text}
    {count === 0 ? "" : count}
</button>

<style>
    button {
        padding: 10px 20px;
        font-size: 16px;
        cursor: pointer;
        background-color: #007bff;
        color: white;
        border: none;
        border-radius: 5px;
    }
    button:hover {
        background-color: #0056b3;
    }
</style>
