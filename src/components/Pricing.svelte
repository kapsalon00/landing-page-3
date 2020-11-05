<script>
  let pricing = "weekly";
</script>

<style lang="scss">
  .wrapper {
    background-color: rgb(247, 247, 247);
    padding: 30px 10px;
    .button--wrapper {
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      button {
        margin: 10px;
      }
    }
  }
  .card--wrapper {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    .card {
      box-shadow: 10px 10px 23px -5px rgb(211, 211, 211);
      background-color: white;
      margin: 20px;
      width: 70%;
      padding: 10px 10px 10px 30px;
      max-width: 200px;
      max-height: 420px;

      button {
        width: 100px;
        height: 40px;
        background-color: rgb(73, 123, 197);
        border-color: rgb(73, 123, 197);
        color: white;
        &:hover {
          background-color: rgb(54, 54, 54);
          border-color: rgb(54, 54, 54);
          color: white;
        }
      }
    }
  }
  .button-active {
    width: 100px;
    height: 40px;
    background-color: rgb(54, 54, 54) !important;
    color: white !important;
    cursor: pointer !important;
  }
  .button {
    width: 100px;
    height: 40px;
    background-color: rgb(247, 247, 247);
    border-color: rgb(247, 247, 247);
    color: rgb(54, 54, 54);
    cursor: pointer;
  }
  @media (min-width: 960px) {
    .card--wrapper {
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
    }
  }
</style>

<div class="wrapper">
  <h1 data-aos="zoom-in" style="text-align:center;">Pricing Plans</h1>
  <div class="button--wrapper">
    <button
      class="button"
      class:button-active={pricing == 'weekly'}
      on:click={() => (pricing = 'weekly')}>WEEKLY</button>
    <button
      class="button"
      class:button-active={pricing == 'monthly'}
      on:click={() => (pricing = 'monthly')}>MONTHLY</button>
  </div>
  {#if pricing == 'weekly'}
    <div class="card--wrapper">
      <div data-aos="zoom-in-up" class="card">
        <h1>Basic</h1>
        <h1>Free</h1>
        <p>100MB Disk Space</p>
        <p>2 Sub Domains</p>
        <p>5 Email Accounts</p>
        <p>24/7 support</p>
        <button>Select</button>
      </div>

      <div data-aos="zoom-in-up" class="card">
        <h1>Standard</h1>
        <h1>$30/week</h1>
        <p>100MB Disk Space</p>
        <p>2 Sub Domains</p>
        <p>5 Email Accounts</p>
        <p>24/7 support</p>
        <button>Select</button>
      </div>

      <div data-aos="zoom-in-up" class="card">
        <h1>Business</h1>
        <h1>$90/week</h1>
        <p>100MB Disk Space</p>
        <p>2 Sub Domains</p>
        <p>5 Email Accounts</p>
        <p>24/7 support</p>
        <button>Select</button>
      </div>

      <div data-aos="zoom-in-up" class="card">
        <h1>Basic</h1>
        <h1>$120/week</h1>
        <p>100MB Disk Space</p>
        <p>2 Sub Domains</p>
        <p>5 Email Accounts</p>
        <p>24/7 support</p>
        <button>Select</button>
      </div>
    </div>
  {/if}

  {#if pricing == 'monthly'}
    <div class="card--wrapper">
      <div data-aos="zoom-in-up" class="card">
        <h1>Basic</h1>
        <h1>Free</h1>
        <p>100MB Disk Space</p>
        <p>2 Sub Domains</p>
        <p>5 Email Accounts</p>
        <p>24/7 support</p>
        <button>Select</button>
      </div>

      <div data-aos="zoom-in-up" class="card">
        <h1>Standard</h1>
        <h1>$30/mon</h1>
        <p>100MB Disk Space</p>
        <p>2 Sub Domains</p>
        <p>5 Email Accounts</p>
        <p>24/7 support</p>
        <button>Select</button>
      </div>

      <div data-aos="zoom-in-up" class="card">
        <h1>Business</h1>
        <h1>$90/mon</h1>
        <p>100MB Disk Space</p>
        <p>2 Sub Domains</p>
        <p>5 Email Accounts</p>
        <p>24/7 support</p>
        <button>Select</button>
      </div>

      <div data-aos="zoom-in-up" class="card">
        <h1>Basic</h1>
        <h1>$120/mon</h1>
        <p>100MB Disk Space</p>
        <p>2 Sub Domains</p>
        <p>5 Email Accounts</p>
        <p>24/7 support</p>
        <button>Select</button>
      </div>
    </div>
  {/if}
</div>
