<script>
    let count = $state(0);
    const increment = () => {
        count += 1; 
    }
</script>

<button onclick={increment}> 
    Cliqué {count} {count === 1 ? "time" : "times"}
</button>
{#if count > 10}
    <p>{count} is higher than 10</p>
{:else if count < 5}
    <p>{count} is less than 5</p>
{:else}
    <p>{count} is between 0 and 10</p>
{/if}