<script lang="ts">
  import '../app.css';
  import Nav from '$lib/components/Nav.svelte';
  import Footer from '$lib/components/Footer.svelte';

  let { children } = $props();
</script>

<svelte:head>
  <link rel="icon" type="image/svg+xml" href="/favicon.svg" />
</svelte:head>

<Nav />
<main id="main-content">{@render children()}</main>
<Footer />
