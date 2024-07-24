<script>
    export let name;
    export let colors;
</script>


    <h2 class="h2 d-block mb-5 text-center">{name}</h2>
    <div class="pl-5 flex items-center justify-center">
        <div class="box">
            {#each colors as color}
                <div class="p-4" style="background-color: {color};">{color}</div>
            {/each}
        </div>
    </div>

<style>
    .container {
        
    }
    .box {
        border-radius: 5px ;
        overflow: hidden;
        display: grid;
        grid-template-columns: repeat(5, minmax(100px, 1fr));
        gap: 0;
    }
</style>