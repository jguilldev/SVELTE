<script>
    let skills = [
        { id: 1, Name: 'HTML' },
        { id: 2, Name: 'CSS' },
        { id: 3, Name: 'JavaScript' }
    ];
</script>

<div class="skills">
    <h3>Habilidades</h3>
    <ul>
        {#each skills as { id, Name } (id)}
            <li>{Name}</li>
        {/each}
    </ul>
</div>
