<script>
  import Nav from "../components/Nav.svelte";

  export let segment;
</script>

<Nav {segment} />

<section class="section">
  <div class="container">
    <slot />
  </div>
</section>
