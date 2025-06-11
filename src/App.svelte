<script>
  import { Router, Link, Route } from "svelte5-router"
  import Home from "./routes/Home.svelte"
  
  
</script>

<Router>
<!-- Menu -->
  <div>
    <Route path="/" component={Home} />
  </div>
</Router>