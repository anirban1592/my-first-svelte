<div class="body-svelte">
  <nav>
    <a href="/">Home</a>
    <a href="/about">About</a>
  </nav>
  <slot />
</div>

<style>
  nav {
    text-align: center;
  }

  a {
    margin: 15px;
    font-size: 30px;
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  }
</style>
