<script lang="ts">
  import Modal from "./Modal.svelte";
  export let title : string;
  export let SVGpath = "";
  let isModalOpen = false;
  function changeModalState() {
    if (SVGpath !== "") {
      isModalOpen = !isModalOpen;
    }
  }
</script>

<h2 on:click={changeModalState} class={`h2 ${SVGpath ? "h2-dropdown" : ""}`}>
  {title}
  {#if SVGpath !== ""}
    <span class="h2__span">
      <img src={SVGpath} alt="down-arrow" />
    </span>
  {/if}
</h2>
{#if SVGpath !== ""}
  {#if isModalOpen}
    <Modal modalOptions={["History", "Our Team", "Blog"]} />
  {/if}
{/if}

<style>
  .h2 {
    color: var(--almost-black-color);
    cursor: pointer;
    font-size: 1rem;
    padding: 0 1rem;
    font-family: var(--epilogue-font);
    color: var(--medium-gray-color);
  }
  .h2:hover {
    color: var(--almost-black-color);
  }
  .h2-dropdown {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
  }
  .h2__span {
    padding: 0 0 0.2rem 0.5rem;
  }
</style>
