<script>
	export let segment;
</script>

<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" href="https://sapper.svelte.dev/">
      <img src="https://sapper.svelte.dev/sapper-logo-horizontal.svg" width="112" height="28" alt="Sapper">
    </a>
    <a role="button" href="javascript:" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div class="navbar-menu">
    <div class="navbar-end">
      <a href="." class:is-active={segment === undefined} class="navbar-item">
        Home
      </a>
	  <a href="blog" rel=prefetch class:is-active={segment === "blog"} class="navbar-item">
        Blog
      </a>
      <a href="about" class:is-active={segment === "about"} class="navbar-item">
        About
      </a>
    </div>
  </div>
</nav>