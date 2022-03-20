<script>
  import { Router, Route } from 'svelte-routing';
  import Main from './pages/main.svelte';
  import Project from './pages/project.svelte';

  export let url = '';
</script>

<Router {url}>
  <Route path="/project" component={Project} />
  <Route path="/" component={Main} />
</Router>
