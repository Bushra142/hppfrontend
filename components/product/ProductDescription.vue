<template>
  <div class="page-width">
    <div class="zig-zag">
      <div class="left">
        <h2>The Ultimate Packaging Specialist</h2>
        <p>
          We curate encompassing packaging solution for your industrial niche
        </p>
        <img src="~/assets/images/leftimage.png" alt="Whatever" />
      </div>
      <div class="right">
        <p>
          OThe Quality and Alluring Packaging of Custom Wine Gift Boxes Wine is
          a drink that is a part of many people's daily routine, and they love
          to sip it with their favorite people around. Wines are an expensive
          commodity and can also be presented as a gift to loved ones. A wine
          gift box is perfect for giving your wind products on special
          occasions.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductDescription",
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