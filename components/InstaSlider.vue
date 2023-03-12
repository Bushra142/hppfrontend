<template>
  <div class="page-width">
    <div class="insta-slider">
      <h2>
        Find our works
        <span class="color-gray">on Instagram</span>
      </h2>
      <client-only>
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

        <VueSlickCarousel ref="carouselInsta" v-bind="slickOptions">
          <div class="insta-slide">
            <nuxt-link to="/" draggable="false">
              <img
                src="~/assets/images/card.webp"
                alt="Card"
                draggable="false"
              />
            </nuxt-link>
          </div>
          <div class="insta-slide">
            <nuxt-link to="/" draggable="false">
              <img
                src="~/assets/images/card.webp"
                alt="Card"
                draggable="false"
              />
            </nuxt-link>
          </div>
          <div class="insta-slide">
            <nuxt-link to="/" draggable="false">
              <img
                src="~/assets/images/card.webp"
                alt="Card"
                draggable="false"
              />
            </nuxt-link>
          </div>
          <div class="insta-slide">
            <nuxt-link to="/" draggable="false">
              <img
                src="~/assets/images/card.webp"
                alt="Card"
                draggable="false"
              />
            </nuxt-link>
          </div>
          <div class="insta-slide">
            <nuxt-link to="/" draggable="false">
              <img
                src="~/assets/images/card.webp"
                alt="Card"
                draggable="false"
              />
            </nuxt-link>
          </div>
          <div class="insta-slide">
            <nuxt-link to="/" draggable="false">
              <img
                src="~/assets/images/card.webp"
                alt="Card"
                draggable="false"
              />
            </nuxt-link>
          </div>
          <div class="insta-slide">
            <nuxt-link to="/" draggable="false">
              <img
                src="~/assets/images/card.webp"
                alt="Card"
                draggable="false"
              />
            </nuxt-link>
          </div>
          <div class="insta-slide">
            <nuxt-link to="/" draggable="false">
              <img
                src="~/assets/images/card.webp"
                alt="Card"
                draggable="false"
              />
            </nuxt-link>
          </div>
        </VueSlickCarousel>
      </client-only>
    </div>
  </div>
</template>

<script>
export default {
  name: "InstaSlider",
  data() {
    return {
      slickOptions: {
        slidesToShow: 4,
        centerMode: true,
        adaptiveHeight: true,
        arrows: false,
        infinite: true,
        variableWidth: false,
      },
    };
  },
  methods: {
    next() {
      this.$refs.carouselInsta.next();
    },

    previous() {
      this.$refs.carouselInsta.prev();
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