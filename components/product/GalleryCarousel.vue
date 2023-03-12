<template>
  <div class="page-width">
    <div class="gallery-carousel">
      <div class="gallery-part">
        <client-only>
          <VueSlickCarousel
            ref="mainImage"
            :asNavFor="$refs.thumbImages"
            :fade="true"
            :adaptiveHeight="true"
            :focusOnSelect="true"
            :centerMode="true"
            class="mainImage"
          >
            <div class="main-slide">
              <img src="~/assets/images/s1.png" alt="Hello" draggable="false" />
            </div>
            <div class="main-slide">
              <img src="~/assets/images/s2.png" alt="Hello" draggable="false" />
            </div>
            <div class="main-slide">
              <img src="~/assets/images/s3.png" alt="Hello" draggable="false" />
            </div>
            <div class="main-slide">
              <img src="~/assets/images/s4.png" alt="Hello" draggable="false" />
            </div>
            <div class="main-slide">
              <img src="~/assets/images/s5.png" alt="Hello" draggable="false" />
            </div>
            <div class="main-slide">
              <img src="~/assets/images/s6.png" alt="Hello" draggable="false" />
            </div>
          </VueSlickCarousel>
          <VueSlickCarousel
            ref="thumbImages"
            :asNavFor="$refs.mainImage"
            :slidesToShow="4"
            :dots="true"
            :adaptiveHeight="true"
            :focusOnSelect="true"
            class="thumbImages"
          >
            <div class="thumb-slide">
              <img src="~/assets/images/s1.png" alt="Hello" draggable="false" />
            </div>
            <div class="thumb-slide">
              <img src="~/assets/images/s2.png" alt="Hello" draggable="false" />
            </div>
            <div class="thumb-slide">
              <img src="~/assets/images/s3.png" alt="Hello" draggable="false" />
            </div>
            <div class="thumb-slide">
              <img src="~/assets/images/s4.png" alt="Hello" draggable="false" />
            </div>
            <div class="thumb-slide">
              <img src="~/assets/images/s5.png" alt="Hello" draggable="false" />
            </div>
            <div class="thumb-slide">
              <img src="~/assets/images/s6.png" alt="Hello" draggable="false" />
            </div>
          </VueSlickCarousel>
        </client-only>
      </div>
      <div class="form-part">
        <div class="usps">
          <b-card no-body>
            <b-tabs pills card v-model="tabIndex">
              <b-tab title="1. Project Info" active
                ><b-card-text>
                  <div class="text-right">
                    <a href="#!" @click="tabIndex++" class="cta-primary m-3"
                      >Proceed</a
                    >
                  </div>
                </b-card-text></b-tab
              >
              <b-tab title="2. Contact Info"
                ><b-card-text>aaaaa</b-card-text></b-tab
              >
            </b-tabs>
          </b-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "GalleryCarousel",
  data() {
    return {
      tabIndex: 0,
      slickOptions: {
        //slidesToShow: 1,
        //slidesToScroll: 1,
        //arrows: true,
        fade: true,
        adaptiveHeight: true,
        centerMode: true,

        focusOnSelect: true,
      },
      // slickOptions: {
      //   slidesToShow: 1,
      //   centerMode: true,
      //   adaptiveHeight: true,
      //   arrows: false,
      //   infinite: true,
      //   variableWidth: false,
      // },
      slickOptions2: {
        slidesToShow: 4,
        //slidesToScroll: 1,
        dots: true,
        //arrows: true,
        // autoplay: false,
        // speed: 2000,
        //infinite: false,
        cssEase: "linear",
        focusOnSelect: true,
        asNavFor: this.$refs.mainImage,
        adaptiveHeight: true,
        // responsive: [
        //   {
        //     breakpoint: 1200,
        //     settings: {
        //       slidesToShow: 3,
        //       slidesToScroll: 1,
        //     },
        //   },
        //   {
        //     breakpoint: 991,
        //     settings: {
        //       slidesToShow: 4,
        //       slidesToScroll: 1,
        //     },
        //   },
        // ],
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.gallery-carousel {
  display: flex;
  gap: 30px;
  .gallery-part {
    flex-basis: 60%;
    background: #f3f3f3;
    border-radius: 20px;
    overflow: hidden;
    padding: 50px;
    .thumbImages {
      margin-top: 30px;
    }
  }
  .form-part {
    flex-basis: 40%;
  }
}

.main-slide {
  img {
    width: 100%;
    width: 450px;
    margin-left: auto;
    margin-right: auto;
  }
}

.thumb-slide {
  padding: 10px;
  img {
    border-radius: 10px;
    // width: 80px;
    height: 150px;
    width: 100%;
    object-fit: cover;
  }
}
</style>