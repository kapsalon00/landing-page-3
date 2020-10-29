<script>
</script>

<style lang="scss">
  .wrapper {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .left,
  .right {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 10px;
    .text {
      p {
        color: rgb(131, 131, 131);
      }
    }
  }
  .image {
    width: 100%;
    height: 100%;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
</style>

<div class="wrapper">
  <div class="left">
    <div data-aos="fade-right" class="text">
      <h1>Excepteur sint occaecat non lorem proident, sunt in culpa quis.</h1>
      <p>
        Morbi tincidunt nisi tortor, iaculis maximus eros vestibulum at. Ut
        pulvinar tortor non augue fringilla, fermentum consequat nisi rutrum.
        Orci varius natoque penatibus et magnis dis parturient montes, nascetur.
        Nullam luctus hendrerit sapien, sed dictum est. mattis egestas. Morbi
        tincidunt nisi tortor, iaculis maximus eros vestibulum at. Ut pulvinar
        tortor non augue fringilla, fermentum consequat nisi rutrum. Orci varius
        natoque penatibus et magnis dis parturient montes.
      </p>
    </div>
    <div data-aos="fade-left" class="image">
      <img src="assets/trees1.jpg" alt="wave" />
    </div>
  </div>
  <div class="right">
    <div data-aos="fade-right" class="image">
      <img src="assets/trees2.jpg" alt="sky" />
    </div>
    <div data-aos="fade-left" class="text">
      <h1>Excepteur sint occaecat non lorem proident, sunt in culpa quis.</h1>
      <p>
        Morbi tincidunt nisi tortor, iaculis maximus eros vestibulum at. Ut
        pulvinar tortor non augue fringilla, fermentum consequat nisi rutrum.
        Orci varius natoque penatibus et magnis dis parturient montes, nascetur.
        Nullam luctus hendrerit sapien, sed dictum est. mattis egestas. Morbi
        tincidunt nisi tortor, iaculis maximus eros vestibulum at. Ut pulvinar
        tortor non augue fringilla, fermentum consequat nisi rutrum. Orci varius
        natoque penatibus et magnis dis parturient montes.
      </p>
    </div>
  </div>
</div>
