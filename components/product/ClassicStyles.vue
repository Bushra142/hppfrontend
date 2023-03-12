<template>
  <div class="page-width">
    <div class="classic-styles">
      <h2>
        Available in
        <span class="color-gray">4 Classic Styles</span>
      </h2>
      <p>
        Find the perfect packaging solutions tailored to your industry niche.
      </p>
      <div class="boxes">
        <div class="box">
          <img src="~/assets/images/box1.png" alt="Box 1 image" />
          <p>
            Give your packages a branded and personalized touch with custom
            Tissue Paper. With low minimums.
          </p>
        </div>
        <div class="box">
          <img src="~/assets/images/box2.png" alt="Box 2 image" />
          <p>
            Give your packages a branded and personalized touch with custom
            Tissue Paper. With low minimums.
          </p>
        </div>
        <div class="box">
          <img src="~/assets/images/box3.png" alt="Box 3 image" />
          <p>
            Give your packages a branded and personalized touch with custom
            Tissue Paper. With low minimums.
          </p>
        </div>
        <div class="box">
          <img src="~/assets/images/box4.png" alt="Box 4 image" />
          <p>
            Give your packages a branded and personalized touch with custom
            Tissue Paper. With low minimums.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ClassicStyles",
};
</script>

<style lang="scss" scoped>
.classic-styles {
  margin-top: 50px;
  margin-bottom: 50px;
  > p {
    margin-bottom: 50px;
  }
  .boxes {
    display: flex;
    gap: 30px;
    .box {
      flex-basis: 25%;
      text-align: center;
      img {
        height: 100px;
        width: 100%;
        object-fit: contain;
      }
      p {
        font-family: 14px;
        margin-top: 25px;
      }
    }
  }
}
</style>