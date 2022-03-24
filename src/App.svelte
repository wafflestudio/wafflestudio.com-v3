<script lang="ts">
  import { Router, Route } from 'svelte-routing';
  import Main from './pages/main.svelte';
  import Project from './pages/services.svelte';

  export let url = '';
</script>

<Router {url}>
  <Route path="/services" component={Project} />
  <Route path="/" component={Main} />
</Router>
