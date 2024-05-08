<script lang="ts">
    export let someColor = 'green'
    const changeColor = () => {
        if (someColor === 'blue')
            someColor = 'yellow'
        else {
            someColor = 'blue'
        }
    }
</script>
<h2 style="color: {someColor}">Svelte rocks!</h2>
<button on:click={()=>changeColor()}>Change Color</button>