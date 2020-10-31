<script>
  import MdMenu from "svelte-icons/md/MdMenu.svelte";
  import DiBackbone from "svelte-icons/di/DiBackbone.svelte";

  let width;
  let isOpen = false;
</script>

<style lang="scss">
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px;
    background-color: rgb(102, 128, 167);
  }
  .logo {
    width: 50px;
    height: 50px;
    color: white;
  }
  .hamburger {
    width: 50px;
    height: 50px;
  }

  .modal {
    display: block;
    position: fixed;
    z-index: 1;
    padding-top: 100px;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    overflow: auto;
    background-color: rgb(0, 0, 0);
    background-color: rgba(0, 0, 0, 0.4);
  }

  .modal-content {
    background-color: #fefefe;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #888;
    width: 320px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  @media (min-width: 960px) {
    a {
      text-decoration: none;
      color: white;
      margin: 0 10px;
      &:hover {
        border-bottom: 1px solid white;
        border-top: 1px solid white;
      }
    }
  }
</style>

<svelte:window bind:outerWidth={width} />

<div class="navbar">
  <div class="logo">
    <DiBackbone />
  </div>
  {#if width < 960}
    <div class="hamburger" on:click={() => (isOpen = true)}>
      <MdMenu />
    </div>
    {#if isOpen}
      <div class="modal">
        <div class="modal-content">
          <a href="/">Home</a>
          <a href="/">Why Choose Us</a>
          <a href="/">Overview</a>
          <a href="/">Pricing</a>
          <a href="/">Faq's</a>
          <a href="/">Contact</a>
          <a href="/">Login</a>
        </div>
      </div>
    {/if}
  {:else}
    <div class="links-wrapper">
      <a href="/">Home</a>
      <a href="/">Why Choose Us</a>
      <a href="/">Overview</a>
      <a href="/">Pricing</a>
      <a href="/">Faq's</a>
      <a href="/">Contact</a>
      <a href="/">Login</a>
    </div>
  {/if}
</div>
