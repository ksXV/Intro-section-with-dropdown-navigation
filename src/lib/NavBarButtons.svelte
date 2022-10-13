<div class="div">
  <button class="div__button div__button--no-border">Login</button>
  <button class="div__button div__button--register">Register</button>
</div>

<style>
  .div {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }
  .div__button {
    font-family: var(--epilogue-font);
    background-color: var(--white-color);
    color: var(--medium-gray-color);
    cursor: pointer;
    padding: 0.75rem 1rem;
    margin: 0 0.5rem;
  }
  .div__button--no-border {
    border: 0;
  }
  .div__button--register {
    border: 2px solid var(--medium-gray-color);
    border-radius: 10px;
  }
  .div__button:hover {
    color: var(--almost-black-color);
  }
  .div__button--register:hover {
    border-color: var(--almost-black-color);
  }
</style>
