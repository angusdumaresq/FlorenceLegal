<script>
    import Nav from '$lib/components/Nav.svelte';
    import { goto } from '$app/navigation';

    function viewProducts() {
        goto('/privacyPolicy');
    }
</script>

<Nav />

<section
  class="bg-primary text-white d-flex align-items-center"
  style="height: calc(100vh - 56px);"
>
  <div class="container">
    <div class="row align-items-center">
      <!-- Left side: Image or placeholder div -->
      <div class="col-12 col-md-4 mb-4 mb-md-0">
        <div
          class="bg-light d-flex justify-content-center align-items-center"
          style="height: 100%; min-height: 300px; color: #333;"
        >
          Image Placeholder
        </div>
      </div>

      <!-- Right side: Text and button -->
      <div class="col-12 col-md-8 text-center text-md-start">
        <h1 class="display-4 fw-bold">Welcome to My Hero Page</h1>
        <p class="lead">
          This is some placeholder text describing your products or services.
        </p>
        <button class="btn btn-light btn-lg mt-3" on:click={viewProducts}>
          View Products
        </button>
      </div>
    </div>
  </div>
</section>
