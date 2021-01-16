<script>
  import Router from 'svelte-spa-router'
  import Home from './Home';
  import Add from './App.svelte';
  
  const routes = {
    '/': Home,
    '/add': Add,
    '*': Home
  };

</script>

<main>
  <Router routes={routes}></Router>
</main>

<style>
	main {
                background-color: rgm(255, 251, 246);
                padding: 2em;
                wigth: 100%;
                height: 100%;
		text-align: center;
                overflow-y: auto;
	}
</style>
