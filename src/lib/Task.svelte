<script>
    let {name = "task vide"} = $props();
    let important = "Elle est <strong>importante</strong>"
</script>
<p>{name}, Ceci est ma tâche</p>
<p>{@html important}</p>