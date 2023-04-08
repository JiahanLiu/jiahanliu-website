<!-- App.svelte -->
<script>
	import { Router, Route } from 'svelte-routing';
	import Navigation from './Navigation.svelte';
	import Home from './Home.svelte';
	import About from './About.svelte';
  </script>
  
  <Navigation />
  
  <Router>
	<Route path="/" component={Home} />
	<Route path="/about" component={About} />
  </Router>
  