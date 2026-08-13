<script lang="ts">
  import favicon from "$lib/assets/favicon.svg";

  let { children } = $props();
</script>

<svelte:head>
  <link rel="icon" href={favicon} />

  <meta
    name="color-scheme"
    content="only light"
  />

  <meta
    name="theme-color"
    content="#001d3d"
  />
</svelte:head>

<section id="convite">
  <section id="convite-intro">
    {@render children()}
  </section>
</section>

<style>
  /* =========================================================
     PROTEÇÃO CONTRA DARK MODE
  ========================================================= */

  :global(html) {
    color-scheme: only light !important;
    background: #001d3d !important;
  }

  :global(body) {
    margin: 0;
    min-height: 100vh;

    background: #001d3d !important;
    color: #ffc300 !important;

    color-scheme: only light !important;
  }


  /* =========================================================
     DARK MODE DO DISPOSITIVO
  ========================================================= */

  @media (prefers-color-scheme: dark) {
    :global(html) {
      background: #001d3d !important;
      color-scheme: only light !important;
    }

    :global(body) {
      background: #001d3d !important;
      color: #ffc300 !important;
      color-scheme: only light !important;
    }

    :global(p),
    :global(h1),
    :global(h2),
    :global(h3),
    :global(a) {
      color: #ffc300 !important;
    }
  }


  /* =========================================================
     CORES
  ========================================================= */

  :global(p),
  :global(h1),
  :global(h2),
  :global(h3) {
    color: #ffc300;
  }

  :global(a) {
    color: #ffd60a;
    text-decoration: none;
  }


  /* =========================================================
     CONVITE
  ========================================================= */

  #convite {
    min-height: 100vh;
    padding: 5vw;

    background:
      radial-gradient(
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
      #001d3d !important;
  }


  /* =========================================================
     CONTEÚDO
  ========================================================= */

  #convite-intro {
    display: flex;
    flex-direction: column;
    gap: 160px;

    padding: 5vw;

    border: 2px solid #ffc300;

    text-align: center;
  }
</style>