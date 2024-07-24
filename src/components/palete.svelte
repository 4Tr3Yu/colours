<script>
    export let name;
    export let colors;
</script>
<div class="container">
    <h1>{name}</h1>
    <div class="box">
        {#each colors as color}
            <div class="p-4" style="background-color: {color};">{color}</div>
        {/each}
    </div>
</div>
<style>
    .container {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 1rem;
    }
</style>