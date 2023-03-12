<template>
  <div class="page-width">
    <div class="industry-slider">
      <h2>
        Shop packaging
        <span class="color-gray">solutions by industry needs</span>
      </h2>
      <p>Make the most of your niche with our best collection</p>

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
      <VueSlickCarousel ref="carouselIndustry" v-bind="slickOptions">
        <div class="industry-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/card.webp" alt="Card" draggable="false"  />
            <h4 class="slide-title">Hello</h4>
          </nuxt-link>
        </div>
        <div class="industry-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/card.webp" alt="Card" draggable="false" />
            <h4 class="slide-title">Hello</h4>
          </nuxt-link>
        </div>
        <div class="industry-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/card.webp" alt="Card" draggable="false" />
            <h4 class="slide-title">Hello</h4>
          </nuxt-link>
        </div>
        <div class="industry-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/card.webp" alt="Card" draggable="false" />
            <h4 class="slide-title">Hello</h4>
          </nuxt-link>
        </div>
        <div class="industry-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/card.webp" alt="Card" draggable="false" />
            <h4 class="slide-title">Hello</h4>
          </nuxt-link>
        </div>
        <div class="industry-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/card.webp" alt="Card" draggable="false" />
            <h4 class="slide-title">Hello</h4>
          </nuxt-link>
        </div>
        <div class="industry-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/card.webp" alt="Card" draggable="false" />
            <h4 class="slide-title">Hello</h4>
          </nuxt-link>
        </div>
      </VueSlickCarousel>
    </div>
  </div>
</template>

<script>
export default {
  name: "IndustrySlider",

  data() {
    return {
      slickOptions: {
        slidesToShow: 4.2,
        centerMode: false,
        adaptiveHeight: true,
        arrows: false,
        infinite: false,
        variableWidth: false,
        swipeToSlide: true,
      },
    };
  },
  methods: {
    next() {
      this.$refs.carouselIndustry.next();
    },

    previous() {
      this.$refs.carouselIndustry.prev();
    },
  },
};
</script>

<style lang="scss" scoped>
.industry-slider {
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
.industry-slide {
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
  h4 {
    font-family: "BodyRegular";
    font-size: 18px;
    margin-top: 15px;
  }
}
</style>