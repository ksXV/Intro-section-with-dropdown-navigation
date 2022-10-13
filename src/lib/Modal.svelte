<script>
  export let modalOptions = [];
  export let modalPosition = "";
</script>

<div
  class="div--modal"
  style="top: 5rem;
left: 20.5rem;"
>
  {#each modalOptions as modalOption}
    <h2 class="div--modal__h2">{modalOption}</h2>
  {/each}
</div>

<style>
  .div--modal {
    width: 5.5rem;
    height: 7rem;
    background-color: var(--white-color);
    -webkit-box-shadow: 5px 5px 15px 5px rgba(0, 0, 0, 0.05);
    box-shadow: 5px 5px 15px 5px rgba(0, 0, 0, 0.05);
    position: absolute;
    padding: 0.75rem;
    border-radius: 10%;
  }
  .div--modal__h2 {
    cursor: pointer;
    font-family: var(--epilogue-font);
    font-weight: 500;
    font-size: 0.9rem;
    padding: 0.5rem;
    color: var(--medium-gray-color);
    margin: 0;
  }
</style>
