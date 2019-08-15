<script>
    import { Button } from 'sveltestrap';
	import Actor from './components/Actor.svelte';
	export let name;

	function random() {
		return Math.floor((Math.random() * 10) + 1);
	}

	function handleClick() {
		alert("hola");
	}
</script>

<head>
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
</head>

<style>
	h1 {
		color: purple;
	}
</style>

<h1>Dungeon Master combat tracker!</h1>

<Actor name="von Dersen" iniciative="{random()}"></Actor>
<Actor name="Goblin 1" iniciative="{random()}"></Actor>
<Actor name="Goblin 2" iniciative="{random()}"></Actor>

<Button on:click="{handleClick}" >Next</Button> 
