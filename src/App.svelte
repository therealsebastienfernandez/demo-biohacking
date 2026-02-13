<script lang="ts">
  import Task from "./lib/Task.svelte";
  import Counter from "./lib/Counter.svelte";
  import Points from "./lib/Points.svelte";
  import Timer from "./lib/Timer.svelte";
  import PackageInfo from "./lib/PackageInfo.svelte";
  import Colours from "./lib/Colours.svelte";

  let dashboard = "Menu interactif";
  let todolist = "Liste de tâches";
  const pkg = {
		name: 'svelte',
		version: 5,
		description: 'blazing fast',
		website: 'https://svelte.dev'
	};
</script>

<main>
  <h1>Biohacking personnel</h1>
  <div>
    <h2>{dashboard.toLocaleUpperCase()}</h2>
    <p>Vous pouvez dans le {dashboard} voir vos statistiques</p>
    <Counter />
    <p>Nombre de points : </p>
    <Points />
  </div>
  <div>
    <h2>{todolist.toLocaleUpperCase()}</h2>
    <p>Timer</p>
    <Task name={"sleep"}/>
    <Task name={"workout"}/>
    <Task />
  </div>
  <div>
    <h2>Outils</h2>
    <Timer />
    <PackageInfo {...pkg}/>
    <Colours />
  </div>
</main>

<style>
  h1 {
    color: cyan;
  }
  
</style>
