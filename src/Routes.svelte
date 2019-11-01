<script>
  import { Router, Route } from 'svero';

  import NotFound from './NotFound.svelte';

  import Home from './pages/home/Home.svelte';
  import ProfileDetail from './pages/profile/ProfileDetail.svelte';
</script>

<Router>
  <Route path="*" component={NotFound} />
  <Route path="/" exact component={Home} />
  <Route path="/profile/:username" component={ProfileDetail} />
</Router>
