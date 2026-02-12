<script lang="ts">
  import Task from "./lib/Task.svelte";
  import Counter from "./lib/Counter.svelte";

  let dashboard = "Menu interactif";
  let todolist = "Liste de tâches";
</script>

<main>
  <h1>Biohacking personnel</h1>
  <div>
    <h2>{dashboard.toLocaleUpperCase()}</h2>
    <p>Vous pouvez dans le {dashboard} voir vos statistiques</p>
    <Counter />
  </div>
  <div>
    <h2>{todolist.toLocaleUpperCase()}</h2>
    <Task />
  </div>
</main>

<style>
  h1 {
    color: cyan;
  }
  
</style>
