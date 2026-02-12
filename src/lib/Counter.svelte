<script>
    let count = $state(0);
    const increment = () => {
        count += 1; 
    }
</script>

<button onclick={increment}> 
    Cliqué {count} {count === 1 ? "time" : "times"}
</button>