<script lang="ts">
  import favicon from "$lib/assets/favicon.svg";

  let { children } = $props();
</script>

<svelte:head>
  <link rel="icon" href={favicon} />
</svelte:head>

<section id="convite">
  <section id="convite-intro">
    {@render children()}
  </section>
</section>

<style>
  :global(html) {
    color-scheme: only light;
    background: #001d3d;
  }

  :global(body) {
    margin: 0;
    min-height: 100vh;
    background: #001d3d;
    color: #ffc300;
  }

  :global(*) {
    color-scheme: only light;
  }

  :global(p),
  :global(h1),
  :global(h2),
  :global(h3),
  :global(a) {
    color: #ffc300;
  }

  #convite {
    padding: 5vw;
    background: radial-gradient(
        circle at 20% 15%,
        rgba(0, 53, 102, 1) 0%,
        rgba(0, 53, 102, 0.45) 30%,
        transparent 65%
      ),
      radial-gradient(
        circle at 85% 80%,
        rgba(0, 53, 102, 0.65) 0%,
        transparent 55%
      ),
      radial-gradient(
        circle at 50% 50%,
        rgba(0, 29, 61, 0.4) 0%,
        transparent 70%
      ),
      #001d3d;
  }

  #convite-intro {
    border: 2px solid #ffc300;
    padding: 5vw;
    display: flex;
    flex-direction: column;
    text-align: center;
    gap: 160px;
  }
</style>
