<template>
  <div class="page-width">
    <div class="home-hero">
      <div class="text-part">
        <h1>
          Make an impact in 2023
          <span>with easily customizable, sustainable packaging.</span>
        </h1>
        <a href="#!" class="cta-primary">Order Packaging</a>
        <div class="clients">
          <p class="tagline color-primary">
            TRUSTED BY OVER 50,000 COMPANIES LIKE:
          </p>
          <div class="client-logos">
            <img src="~/assets/images/samsung.svg" alt="Samsung logo" />
            <img src="~/assets/images/citrix.svg" alt="Citrix logo" />
            <img src="~/assets/images/telogis.svg" alt="Telogis logo" />
            <img src="~/assets/images/loews.svg" alt="Loews logo" />
            <img src="~/assets/images/netflix.svg" alt="Netflix logo" />
          </div>
        </div>
      </div>
      <div class="image-part">
        <img src="~/assets/images/boxes.webp" alt="HPP Hero" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style lang="scss" scoped>
.home-hero {
  background: #f2f2f2;
  border-radius: 20px;
  // height: calc(100vh - 232px);
  height: 80vh;
  display: flex;
  padding: 50px;
  .text-part {
    flex-basis: 50%;
    height: 100%;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: start;
    position: relative;
    h1 {
      line-height: 1em;
      span {
        display: block;
        font-size: 18px;
      }
    }
    .cta-primary {
      margin-top: 15px;
    }
    .clients {
      position: absolute;
      bottom: -25px;
      .client-logos {
        display: flex;
        gap: 30px;
        align-items: center;
        img {
          filter: grayscale(1);
          height: 30px;
          width: 100%;
          max-width: 150px;
          object-fit: contain;
        }
      }
    }
  }
  .image-part {
    flex-basis: 50%;
    display: flex;
    align-items: center;
    img {
      width: 100%;
    }
  }
}
</style>