<script>
  import FaUserFriends from "svelte-icons/fa/FaUserFriends.svelte";
  import FaStar from "svelte-icons/fa/FaStar.svelte";
  import { fly, fade } from "svelte/transition";
  import { onDestroy, onMount } from "svelte";

  let panel = 1;
  let interval;
  onMount(() => {
    interval = setInterval(() => {
      if (panel < 3) {
        panel++;
      } else {
        panel = 1;
      }
    }, 5000);
  });
  onDestroy(() => {
    clearInterval(interval);
  });
</script>

<style lang="scss">
  .wrapper {
    background-color: rgb(247, 247, 247);
    padding: 10px;
    .left {
      color: rgb(73, 123, 197);
    }
  }

  .stars-wrapper {
    width: 100px;
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    .star {
      color: lightskyblue;
    }
  }
  .dots {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    .dot {
      margin: 10px;
      background-color: grey;
      width: 20px;
      height: 20px;
      border-radius: 50%;
    }
  }
  .active {
    background-color: black !important;
  }
  @media (min-width: 960px) {
    .container {
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      .left {
        width: 50%;
        .image {
          height: 400px;
          width: 400px;
          margin: 0 auto;
        }
      }
      .right {
        width: 50%;
        .card {
          height: 400px;
          width: 400px;
          padding-top: 50px;
        }
      }
    }
  }
</style>

<div class="wrapper">
  <h1 style="text-align:center;">Honorable Clients</h1>
  <div class="container">
    <div class="left">
      <div class="image">
        <FaUserFriends />
      </div>
    </div>
    <div class="right">
      {#if panel == 1}
        <div in:fade class="card">
          <h1>John Random</h1>
          <h2>- lorem</h2>
          <div class="stars-wrapper">
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
          </div>
          <p>
            &quot; Donec rutrum congue leo eget consectetur sed, convallis at
            tellus. Nulla quis lorem ut libero malesuada feugiat.Nulla quis
            lorem ut libero malesuada feugiat. Donec rutrum congue leo eget
            malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit
          </p>
        </div>
      {:else if panel == 2}
        <div in:fade class="card">
          <h1>Rave Random</h1>
          <h2>- ipsum</h2>
          <div class="stars-wrapper">
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
          </div>
          <p>
            &quot; Donec rutrum congue leo eget consectetur sed, convallis at
            tellus. Nulla quis lorem ut libero malesuada feugiat.Nulla quis
            lorem ut libero malesuada feugiat. Donec rutrum congue leo eget
            malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit
          </p>
        </div>
      {:else}
        <div in:fade class="card">
          <h1>Katey Random</h1>
          <h2>- dolor</h2>
          <div class="stars-wrapper">
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
            <div class="star">
              <FaStar />
            </div>
          </div>
          <p>
            &quot; Donec rutrum congue leo eget consectetur sed, convallis at
            tellus. Nulla quis lorem ut libero malesuada feugiat.Nulla quis
            lorem ut libero malesuada feugiat. Donec rutrum congue leo eget
            malesuada. Lorem ipsum dolor sit amet, consectetur adipiscing elit
          </p>
        </div>
      {/if}
      <div class="dots">
        <div
          class:active={panel == 1}
          on:click={() => (panel = 1)}
          class="dot" />
        <div
          on:click={() => (panel = 2)}
          class:active={panel == 2}
          class="dot" />
        <div
          class:active={panel == 3}
          on:click={() => (panel = 3)}
          class="dot" />
      </div>
    </div>
  </div>
</div>
