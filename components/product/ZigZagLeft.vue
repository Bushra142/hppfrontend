<template>
  <div class="page-width">
    <div class="zig-zag">
      <div class="left">
        <img src="~/assets/images/leftimage.png" alt="Whatever" />
      </div>
      <div class="right">
        <h2>
          10 Corporate Christmas Cards Ideas to send an Awesome Message this
          Year
        </h2>
        <p>
          Our wide collection of premium quality eco-friendly packaging
          materials offers different strengths, looks, and textures to create
          versatile packaging boxes for your custom packaging needs
        </p>
        <a href="#!" class="cta-primary mt-5">Read More</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ZigZagLeft",
};
</script>

<style lang="scss" scoped>
.zig-zag {
  display: flex;
  margin-top: 50px;
  margin-bottom: 50px;
  .left {
    flex-basis: 50%;
    img {
      width: 100%;
      height: auto;
      object-fit: cover;
      border-radius: 20px;
    }
  }
  .right {
    flex-basis: 50%;
    padding: 50px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
  }
}
</style>