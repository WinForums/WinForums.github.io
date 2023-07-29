<script lang="ts">
  import TailwindCss from "./TailwindCSS.svelte";
  import Login from "./lib/pagestuff/Login.svelte";
  import { Link, Route, Router, navigate } from "svelte-routing";
</script>

<main>
  <TailwindCss />
  <Router url="">
    <Route path="/" />
    <Route path="/login"><Login /></Route>
  </Router>
</main>
