<template>
  <div class="categoryslider-parent">
    <div class="category-slider page-width">
      <h2 class="text-center">
        Browse Our
        <span class="color-gray">Categories</span>
      </h2>

      <VueSlickCarousel ref="carouselInsta" v-bind="slickOptions">
        <div class="category-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/category.png" alt="Card" draggable="false" />
            <h4 class="slide-title">Tobacco and Weed Packaging</h4>
          </nuxt-link>
        </div>
        <div class="category-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/category.png" alt="Card" draggable="false" />
            <h4 class="slide-title">Tobacco and Weed Packaging</h4>
          </nuxt-link>
        </div>
        <div class="category-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/category.png" alt="Card" draggable="false" />
            <h4 class="slide-title">Fashion & Apparel</h4>
          </nuxt-link>
        </div>
        <div class="category-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/category.png" alt="Card" draggable="false" />
            <h4 class="slide-title">Tobacco and Weed Packaging</h4>
          </nuxt-link>
        </div>
        <div class="category-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/category.png" alt="Card" draggable="false" />
            <h4 class="slide-title">Tobacco and Weed Packaging</h4>
          </nuxt-link>
        </div>
        <div class="category-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/category.png" alt="Card" draggable="false" />
            <h4 class="slide-title">Tobacco and Weed Packaging</h4>
          </nuxt-link>
        </div>
        <div class="category-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/category.png" alt="Card" draggable="false" />
            <h4 class="slide-title">Tobacco and Weed Packaging</h4>
          </nuxt-link>
        </div>
        <div class="category-slide">
          <nuxt-link to="/" draggable="false">
            <img src="~/assets/images/category.png" alt="Card" draggable="false" />
            <h4 class="slide-title">Tobacco and Weed Packaging</h4>
          </nuxt-link>
        </div>
      </VueSlickCarousel>
    </div>
  </div>
</template>

<script>
export default {
  name: "CategorySlider",
  data() {
    return {
      flickityOptions: {
        adaptiveHeight: true,
        prevNextButtons: true,
        pageDots: false,
        wrapAround: true,
        groupCells: 3,
      },

      slickOptions: {
        slidesToShow: 5.5,
        centerMode: true,
        adaptiveHeight: true,
        arrows: true,
        infinite: true,
        variableWidth: false,
      },
    };
  },
  methods: {
    next() {
      this.$refs.carouselCateg.next();
    },

    previous() {
      this.$refs.carouselCateg.prev();
    },
  },
};
</script>

<style lang="scss" scoped>
.categoryslider-parent {
  background: #f7f7f7;
  margin-top: 50px;
  margin-bottom: 50px;
  padding-top: 50px;
  padding-bottom: 50px;
}
.category-slider {
  > h2 {
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
.category-slide {
  margin-right: 20px;
  margin-left: 20px;
  width: 250px;
  a {
    color: inherit;
    text-decoration: none;
    text-align: center;
  }
  img {
    width: 100%;
    height: 80px;
    object-fit: contain;
  }
  h4 {
    font-family: "BodyRegular";
    font-size: 18px;
    margin-top: 15px;
  }
}
</style>