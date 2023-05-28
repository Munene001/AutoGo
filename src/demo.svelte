<!-- App.svelte -->
<script>
    import { Router, Link, Route } from "svelte-routing";
    import Tailwind from "./lib/tailwind.svelte";
    import Landing from "./lib/landing.svelte";
      import Blog from "./lib/blog.svelte";
      import Listing from "./lib/listing.svelte";
      import Contact from "./lib/contact.svelte";
    export let url = "";
  
  </script>
  
  <Tailwind />
  
  <Router {url}>
    <div>
      <!-- <Route path="blog/:id" component="{BlogPost}" /> -->
      <!-- <Route path="blog" component="{Blog}" /> -->
      <!-- <Route path="about" component="{About}" /> -->
      <Route path="/"><Landing /></Route>
      <Route path="/contact"><Contact /></Route>
      <Route path="/blog"><Blog /></Route>
      <Route path="/listing"><Listing /></Route>
    </div>
  </Router>