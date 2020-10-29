<script>
  import MdMenu from "svelte-icons/md/MdMenu.svelte";
  import DiBackbone from "svelte-icons/di/DiBackbone.svelte";
  let isMobile = true;
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
  }
  .hamburger {
    width: 50px;
    height: 50px;
  }
</style>

<div class="navbar">
  <div class="logo">
    <DiBackbone />
  </div>
  {#if isMobile}
    <div class="hamburger">
      <MdMenu />
    </div>
  {:else}
    <div class="links-wrapper">
      <a href="/">Link1</a>
      <a href="/">Link2</a>
      <a href="/">Link3</a>
    </div>
  {/if}
</div>
