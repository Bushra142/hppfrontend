<template>
  <div class="page-width">
    <div class="l1-header">
      <div class="left-side">
        <h1 class="h2">CBD & Tobacco Packaging</h1>
        <p>
          Make your product feel like a gift for your customers with our custom
          tissue paper. Unlike many wrapping papers, our eco-friendly tissue
          paper is 100% circular and can be composted or recycled after use.
          Build your unboxing experience in style without worrying about the
          impact.
        </p>
        <img src="~/assets/images/cbd.webp" alt="Product image" />
      </div>
      <div class="right-side">
        <h2>Get a Custom Quote</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "LThreeHeader",
  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
.l1-header {
  background: #f7f7f7;
  border-radius: 20px;
  padding: 50px;
  display: flex;
  .left-side {
    flex-basis: 60%;
    p {
      margin-top: 20px;
      width: 80%;
    }
    img {
      margin-top: 20px;
      width: 70%;
    }
    .select-box {
      margin-top: 30px;
    }
  }
  .right-side {
    flex-basis: 40%;
  }
}
</style>