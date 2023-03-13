<script lang="ts">
  import { Router, Route } from "svelte-routing";

  import HomePage from "./pages/home/HomePage.svelte";
  import AdoraPage from "./pages/adora/AdoraPage.svelte";
  import UnderConstruction from "./pages/under-construction/UnderConstruction.svelte";

  export let url = window.location.pathname;

  const isProduction = process.env.NODE_ENV == "production";
</script>

{#if !isProduction}
  <UnderConstruction />
{:else}
  <Router basepath="" {url}>
    <Route path="/adora" component={AdoraPage} />
    <Route path="/"><HomePage /></Route>
  </Router>
{/if}
