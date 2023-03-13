<script lang="ts">
  import { Router, Route } from "svelte-routing";

  import HomePage from "./pages/home/HomePage.svelte";
  import AdoraPage from "./pages/adora/AdoraPage.svelte";

  export let url = window.location.pathname;
</script>

<Router basepath="" {url}>
  <Route path="/adora" component={AdoraPage} />
  <Route path="/"><HomePage /></Route>
</Router>
