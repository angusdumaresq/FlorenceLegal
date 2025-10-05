<script>
    import Nav from '$lib/components/Nav.svelte';
    import HeroLogo from '$lib/icons/HeroLogo.svelte';
    import { goto } from '$app/navigation';
	import Footer from '$lib/components/Footer.svelte';

    function viewProducts() {
        goto('/privacy-policy');
    }
</script>

<Nav />

<section class="landing d-flex flex-column justify-content-center align-items-center">
    <div class="hero-logo">
        <HeroLogo />
    </div>

    <button class="btn btn-primary btn-md mt-4" on:click={viewProducts}>
        Discord Expected Value Bot
    </button>
</section>

<Footer />

<style>
  .landing {
    height: calc(100vh - 56px); 
    background-color: #ffffff; 
    color: #333;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .hero-logo {
    width: 100%;
    max-width: 500px;
    margin-bottom: 2rem;
    transform: scale(1.5);
  }

  button {
    padding: 1rem 2rem;
    font-size: 1.25rem;
    transition: transform 0.2s;
  }

  button:hover {
    transform: scale(1.05);
  }
</style>
