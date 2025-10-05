<script>
  import FMLogo from "$lib/icons/FMLogo.svelte";
</script>

<nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="fm-logo navbar-brand d-flex align-items-center" href="/">
      <FMLogo />
    </a>

    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarText" aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarText">
      <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
        <li class="nav-item mx-2">
          <a class="nav-link" href="#">About</a>
        </li>
        <li class="nav-item mx-2">
          <a class="nav-link" href="#">Products</a>
        </li>
      </ul>
    </div>
  </div>
</nav>

<style>
  .fm-logo {
    width: 52px; 
    height: auto;
  }

  .navbar-brand {
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }
</style>
