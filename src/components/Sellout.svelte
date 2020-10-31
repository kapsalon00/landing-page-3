<script>
  import MdBlurOn from "svelte-icons/md/MdBlurOn.svelte";
  import MdDoneAll from "svelte-icons/md/MdDoneAll.svelte";
  import MdEuroSymbol from "svelte-icons/md/MdEuroSymbol.svelte";
</script>

<style lang="scss">
  .wrapper {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 50px;
    h1 {
      margin: 14px 0;
      color: rgb(77, 77, 77);
    }
    p {
      margin: 8px 0;
      color: rgb(122, 122, 122);
      line-height: 32px;
    }
  }
  .card {
    box-shadow: 10px 10px 23px -5px rgb(211, 211, 211);
    width: 85%;
    margin: 15px;
    padding: 10px;
    .img {
      width: 35px;
      height: 35px;
      background-color: rgb(245, 245, 245);
      padding: 15px;
    }
    .a {
      color: crimson;
    }
    .b {
      color: lightskyblue;
    }
    .c {
      color: lightgreen;
    }
  }
  @media (min-width: 960px) {
    .container {
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
    }
  }
</style>

<div class="wrapper">
  <h1 data-aos="fade-up">Why choose us?</h1>
  <div class="container">
    <div data-aos="fade-right" class="card">
      <div class="img a">
        <MdBlurOn />
      </div>
      <h1>Fresh</h1>
      <p>
        Excepteur sint occaecat non proident, sunt in culpa quis. Phasellus
        lacinia id erat eu ullamcorper. Nunc id ipsum.
      </p>
    </div>
    <div data-aos="fade-up" class="card">
      <div class="img b">
        <MdDoneAll />
      </div>
      <h1>Design</h1>
      <p>
        Excepteur sint occaecat non proident, sunt in culpa quis. Phasellus
        lacinia id erat eu ullamcorper. Nunc id ipsum.
      </p>
    </div>
    <div data-aos="fade-left" class="card">
      <div class="img c">
        <MdEuroSymbol />
      </div>
      <h1>Safe</h1>
      <p>
        Excepteur sint occaecat non proident, sunt in culpa quis. Phasellus
        lacinia id erat eu ullamcorper. Nunc id ipsum.
      </p>
    </div>
  </div>
</div>
