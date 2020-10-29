<script>
</script>

<style lang="scss">
  .wrapper {
    background-color: lightslategray;
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-size: cover;
  }
  .solutions {
    margin: 60px 0 30px 0;
    width: 90%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    h2 {
      margin: 5px;
    }
    button {
      width: 120px;
      height: 40px;
      margin: 5px;
      background-color: rgb(0, 0, 0, 0);
      color: white;
      border: 2px solid white;
      &:hover {
        border: 2px solid rgb(73, 123, 197);
        color: rgb(73, 123, 197);
      }
    }
  }
  .register {
    margin: 30px 0;
    width: 90%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    input {
      width: 100%;
      background-color: rgb(0, 0, 0, 0);
      padding: 10px;
      color: white;
      &::placeholder {
        color: lightgrey;
      }
    }
    button {
      width: 100%;
      background-color: rgb(102, 128, 167);
      border: 2px solid rgb(102, 128, 167);
      color: white;
      &:hover {
        background-color: rgb(73, 85, 102);
        border: 2px solid rgb(73, 85, 102);
        color: white;
      }
    }
  }
</style>

<div
  class="wrapper"
  style="background: url('assets/bgcc.jpg') no-repeat center center fixed">
  <div class="solutions">
    <h2>Modern Solution -</h2>
    <h2>Lorem Ipsum dolor sit</h2>
    <div class="solutions--wrapper">
      <button>Read More</button>
      <button>Watch Video</button>
    </div>
  </div>
  <div class="register">
    <h1>Register Now</h1>
    <input placeholder="Name" />
    <input placeholder="Email" />
    <input placeholder="Phone Number" />
    <input placeholder="Password" />
    <button>Register Account</button>
  </div>
</div>
