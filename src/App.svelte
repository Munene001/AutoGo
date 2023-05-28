
<script lang="ts">
  import { Router, Link, Route } from "svelte-routing";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
  import CarListing from "./pages/CarListing.svelte";
  import Contact from "./pages/Contact.svelte";

  export let url = "/";
</script>

<Router {url}>
  <div>
    <Route path="/about"><About/></Route>
    <Route path="/contact"><Contact /></Route>
    <Route path="/carlisting"><CarListing/></Route>
     <Route path="/"><Home /></Route>
  </div>
</Router>

