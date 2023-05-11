<script>
  import { Router, Route } from 'svelte-routing'
  import Messages from '../components/Messages.svelte'
  import Settings from '../components/Settings.svelte'

  export let url = '/'
</script>

<Router {url}>
  <div>
    <Route path="/" component={Messages} />
    <Route path="/settings" component={Settings} />
  </div>
</Router>
