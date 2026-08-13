<script lang="ts">
  import favicon from "$lib/assets/favicon.svg";

  let { children } = $props();
</script>

<svelte:head>
  <link rel="icon" href={favicon} />

  <meta name="color-scheme" content="only light" />

  <meta name="theme-color" content="#001d3d" />
</svelte:head>

<section id="convite">
  <svg
    width="100%"
    height="20"
    viewBox="0 0 1000 50"
    preserveAspectRatio="none"
    xmlns="http://www.w3.org/2000/svg"
    fill="none"
    stroke="#ffc300"
    stroke-width="5"
    style="bottom: -4px; position: relative"
  >
    <path d="M 0 50 Q 50 50 50 0 H 950 Q 950 50 1000 50" />
  </svg>
  <section id="convite-intro">
    {@render children()}
  </section>
  <svg
    width="100%"
    height="20"
    viewBox="0 0 1000 50"
    preserveAspectRatio="none"
    xmlns="http://www.w3.org/2000/svg"
    fill="none"
    stroke="#ffc300"
    stroke-width="5"
    style="top: -1px; position: relative"
  >
    <path d="M 0 0 Q 50 0 50 50 H 950 Q 950 0 1000 0" />
  </svg>

  <div id="ondas">
    <div style="display: flex; justify-content: end;">
      <svg
        width="100"
        height="100"
        viewBox="0 0 100 100"
        xmlns="http://www.w3.org/2000/svg"
        fill="#001d3d"
      >
        <path d="M 0 0 Q 50 0 50 50 T 100 100 L 100 0" />
      </svg>
    </div>

    <svg
      width="150"
      height="150"
      viewBox="0 0 100 100"
      xmlns="http://www.w3.org/2000/svg"
      fill="#001d3d"
    >
      <path d="M 0 0 Q 50 0 50 50 T 100 100 L 0 100" />
    </svg>
  </div>
</section>

<style>
  #ondas {
    position: absolute;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    bottom: 0;
    left: 0;
    width: 100vw;
    height: 100%;
    overflow: hidden;
  }

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
    overflow: hidden;
    position: relative;

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
      #001d3d !important;
  }

  /* =========================================================
     CONTEÚDO
  ========================================================= */

  #convite-intro {
    overflow: hidden;
    display: flex;
    flex-direction: column;
    gap: 160px;
    z-index: 1;

    padding: 5vw;

    border-right: 2px solid #e8c44b;
    border-left: 2px solid #e8c44b;

    text-align: center;
  }
</style>
