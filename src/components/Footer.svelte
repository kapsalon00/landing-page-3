<script>
  import DiBackbone from "svelte-icons/di/DiBackbone.svelte";
  import FaTwitter from "svelte-icons/fa/FaTwitter.svelte";
  import FaFacebookF from "svelte-icons/fa/FaFacebookF.svelte";
  import FaLinkedinIn from "svelte-icons/fa/FaLinkedinIn.svelte";
  import FaGooglePlusSquare from "svelte-icons/fa/FaGooglePlusSquare.svelte";
</script>

<style lang="scss">
  .wrapper {
    background-color: rgb(27, 27, 27);
    padding: 10px;
    .up {
      .header {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        color: white;
        .logo {
          width: 30px;
          height: 30px;
        }
      }
      p {
        color: rgb(187, 187, 187);
      }
    }
    .buttons {
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
      .container {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        color: white;
        margin: 10px;
        div {
          width: 30px;
          height: 30px;
          margin-right: 10px;
        }
        button {
          margin: 0;
        }
      }
    }
  }
  .down {
    h1 {
      color: white;
    }
    p {
      color: rgb(187, 187, 187);
    }
    input {
      background-color: rgb(0, 0, 0, 0);
      color: white;
    }
  }

  @media (min-width: 960px) {
    .down {
      display: flex;
      flex-direction: row;
      justify-content: space-evenly;
      align-items: center;
    }
    .address,
    .quick-links,
    .newsletter {
      width: 25%;
      height: 400px;
    }
    .quick-links {
      .container {
        display: flex;
        flex-direction: row;
        .chunk {
          margin: 0 10px;
        }
      }
    }
  }
</style>

<div class="wrapper">
  <div data-aos="zoom-in" class="up">
    <div class="header">
      <div class="logo">
        <DiBackbone />
      </div>
      <h1>Landing</h1>
    </div>
    <p>
      Vivamus magna justo, lacinia eget consectetur sed, convallis at tellus.
      Nulla quis lorem ipnut libero malesuada feugiat. Lorem ipsum dolor sit
      amet, consectetur elit.
    </p>
    <div class="buttons">
      <div class="container">
        <div>
          <FaFacebookF />
        </div>
        <button>facebook</button>
      </div>
      <div class="container">
        <div>
          <FaTwitter />
        </div>
        <button>twitter</button>
      </div>
      <div class="container">
        <div>
          <FaGooglePlusSquare />
        </div>
        <button>google</button>
      </div>
      <div class="container">
        <div>
          <FaLinkedinIn />
        </div>
        <button>linkedin</button>
      </div>
    </div>
  </div>
  <div class="down">
    <div data-aos="fade-right" data-aos-offset="-100" class="address">
      <h1>Address</h1>
      <p>Address : 1234 lock, Charlotte, North Carolina, United States</p>
      <p>Phone : +12 534894364</p>
      <p>Email : info@example.com</p>
      <p>Fax : +12 534894364</p>
    </div>
    <div data-aos="fade-up" data-aos-offset="-100" class="quick-links">
      <h1>Quick Links</h1>
      <div class="container">
        <div class="chunk">
          <p>Why Choose Us</p>
          <p>Overview</p>
          <p>Pricing Plans</p>
          <p>Faq's</p>
          <p>Testimonial</p>
          <p>Contact</p>
        </div>
        <div class="chunk">
          <p>Privacy Policy</p>
          <p>General Terms</p>
          <p>Faq's</p>
          <p>Knowledge</p>
          <p>Forum</p>
        </div>
      </div>
    </div>
    <div data-aos="fade-left" data-aos-offset="-100" class="newsletter">
      <h1>Newsletter</h1>
      <p>
        By subscribing to our mailing list you will always get latest news and
        updates from us.
      </p>
      <input placeholder="Enter your email..." />
    </div>
  </div>
</div>
