<!-- svelte-ignore a11y-img-redundant-alt -->
<script>
  import Logo from "../assets/logo.svg";
  import DownArrow from "../assets/icon-arrow-down.svg";
  import NavBarRoute from "./NavBarRoute.svelte";
  import NavBarButtons from "./NavBarButtons.svelte";
</script>

<nav class="nav nav--flex-row">
  <div class="nav__div">
    <img src={Logo} class="div__image" alt="logo-image" />
    <div class="nav__div">
      <NavBarRoute title={"Features"} SVGpath={DownArrow} />
      <NavBarRoute title={"Company"} SVGpath={DownArrow} />
      <NavBarRoute title={"Careers"} />
      <NavBarRoute title={"About"} />
    </div>
  </div>
  <NavBarButtons />
</nav>

<style>
  .nav {
    border: 1px solid pink;
    padding: 1.5rem 2rem;
    line-height: 1.6;
    margin: 0;
    justify-content: space-between;
  }
  .div__image {
    padding: 0.6rem 1.5rem 0 0;
  }
  .nav--flex-row {
    display: flex;
    flex-direction: row;
    align-items: center;
  }
  .nav__div {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    padding: 0 1.5rem;
  }
</style>
