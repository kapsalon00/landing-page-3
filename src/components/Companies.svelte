<script>
  import DiApple from "svelte-icons/di/DiApple.svelte";
  import DiClojure from "svelte-icons/di/DiClojure.svelte";
  import GoEye from "svelte-icons/go/GoEye.svelte";
  import GoGlobe from "svelte-icons/go/GoGlobe.svelte";
  import GoLightBulb from "svelte-icons/go/GoLightBulb.svelte";
  import GoMarkGithub from "svelte-icons/go/GoMarkGithub.svelte";
</script>

<style lang="scss">
  .wrapper {
    margin: 10px;
    text-align: center;
  }
  .logos-wrapper {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    .logo {
      width: 100px;
      height: 100px;
      margin: 10px;
    }
    .a {
      color: rgb(35, 168, 95);
    }
    .b {
      color: rgb(87, 52, 170);
    }
    .c {
      color: rgb(150, 55, 76);
    }
  }
  @media (min-width: 960px) {
    .logos-wrapper {
      flex-direction: row;
    }
  }
</style>

<div class="wrapper">
  <h2>Trusted by the world's best companies</h2>
  <div class="logos-wrapper">
    <div data-aos="fade-up" class="logo a">
      <DiApple />
    </div>
    <div data-aos="fade-up" class="logo b">
      <DiClojure />
    </div>
    <div data-aos="fade-up" class="logo a">
      <GoEye />
    </div>
    <div data-aos="fade-up" class="logo c">
      <GoGlobe />
    </div>
    <div data-aos="fade-up" class="logo b">
      <GoLightBulb />
    </div>
    <div data-aos="fade-up" class="logo a">
      <GoMarkGithub />
    </div>
  </div>
</div>
