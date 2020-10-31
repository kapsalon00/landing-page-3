<script>
</script>

<style lang="scss">
  .wrapper {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    max-width: 600px;
    margin: 0 auto;
    input,
    textarea {
      width: 80%;
      padding: 12px;
    }
  }
  .primary {
    margin: 10px;
    width: 100px;
    height: 40px;
    background-color: rgb(73, 123, 197);
    border: 1px solid rgb(73, 123, 197);
    color: white;
    cursor: pointer;
    &:hover {
      background-color: rgb(54, 54, 54);
      border: 1px solid rgb(54, 54, 54);
    }
  }
</style>

<div class="wrapper">
  <h1 style="text-align:center;">Get In Touch</h1>
  <input placeholder="First Name" />
  <input placeholder="Last Name" />
  <input placeholder="Email" />
  <input placeholder="Phone Number" />
  <textarea rows="4" placeholder="Message" />
  <button class="primary">Submit</button>
</div>
