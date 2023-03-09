<template>
  <div class="page-width">
    <div class="insta-slider">
      <h2>
        Find our works 
        <span class="color-gray">on Instagram</span>
      </h2>
      <client-only>
        <!-- if you don't want to use the buttons Flickity provides -->
        <div class="flickity-controls">
          <img
            @click="previous()"
            src="~/assets/icons/arrow-left.svg"
            alt="Slide Back"
            class="custom-arrow"
          />
          <img
            @click="next()"
            src="~/assets/icons/arrow-right.svg"
            alt="Slide Next"
            class="custom-arrow"
          />
        </div>
        <flickity ref="flickity" :options="flickityOptions">
          <div class="carousel-cell insta-slide">
            <nuxt-link to="/">
              <img src="~/assets/images/card.webp" alt="Card" />
            </nuxt-link>
          </div>
          <div class="carousel-cell insta-slide">
            <nuxt-link to="/">
              <img src="~/assets/images/card.webp" alt="Card" />
            </nuxt-link>
          </div>
          <div class="carousel-cell insta-slide">
            <nuxt-link to="/">
              <img src="~/assets/images/card.webp" alt="Card" />
            </nuxt-link>
          </div>
          <div class="carousel-cell insta-slide">
            <nuxt-link to="/">
              <img src="~/assets/images/card.webp" alt="Card" />
            </nuxt-link>
          </div>
          <div class="carousel-cell insta-slide">
            <nuxt-link to="/">
              <img src="~/assets/images/card.webp" alt="Card" />
            </nuxt-link>
          </div>
          <div class="carousel-cell insta-slide">
            <nuxt-link to="/">
              <img src="~/assets/images/card.webp" alt="Card" />
            </nuxt-link>
          </div>
          <div class="carousel-cell insta-slide">
            <nuxt-link to="/">
              <img src="~/assets/images/card.webp" alt="Card" />
            </nuxt-link>
          </div>
          <div class="carousel-cell insta-slide">
            <nuxt-link to="/">
              <img src="~/assets/images/card.webp" alt="Card" />
            </nuxt-link>
          </div>
        </flickity>
      </client-only>
    </div>
  </div>
</template>

<script>
export default {
  name: "InstaSlider",
  data() {
    return {
      flickityOptions: {
        adaptiveHeight: true,
        prevNextButtons: false,
        pageDots: false,
        wrapAround: true,
        groupCells: 3,
      },
    };
  },
  methods: {
    next() {
      this.$refs.flickity.next();
    },

    previous() {
      this.$refs.flickity.previous();
    },
  },
};
</script>

<style lang="scss" scoped>
.insta-slider {
  margin-top: 50px;
  margin-bottom: 50px;
  > p {
    margin-bottom: 50px;
  }

  .flickity-controls {
    display: flex;
    justify-content: end;
    gap: 20px;
    margin-bottom: 25px;
    .custom-arrow {
      width: 30px;
    }
  }
}
.insta-slide {
  height: 535px;
  margin-right: 20px;
  a {
    color: inherit;
    text-decoration: none;
  }
  img {
    border-radius: 30px;
    width: 100%;
    filter: drop-shadow(6px 6px 12px rgba(0, 0, 0, 0.12));
    max-width: 300px;
  }
}
</style>