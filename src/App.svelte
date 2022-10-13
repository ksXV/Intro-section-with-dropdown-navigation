<script>
  // @ts-nocheck
  import NavBar from "./lib/NavBar.svelte";
</script>

<main>
  <NavBar />
</main>

<svelte:head>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Epilogue:wght@500;700&display=swap"
    rel="stylesheet"
  />
</svelte:head>

<style>
  :root {
    --white-color: hsl(0, 0%, 98%);
    --medium-gray-color: hsl(0, 0%, 41%);
    --almost-black-color: hsl(0, 0%, 8%);
    --epilogue-font: "Epilogue", sans-serif;
  }
  :global(body) {
    background-color: var(--white-color);
    margin: 0;
  }
  :global(h1, h2, h3) {
    font-size: inherit;
  }
</style>
