<script>
    import Button from "./Button.svelte";
    let contador = 0
    function handleClick(){
        contador+=1;
    }
</script>

<style>

</style>

<div>
    <button on:click={handleClick}>Click {contador}</button> 
    <!-- mediante {} se pued eusar la logica de js como en react o JSX -->

    <Button 
    text = "click" 
    {count}
    on:click={handleClick}/>
</div>