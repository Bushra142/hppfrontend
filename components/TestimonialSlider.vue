<template>
  <div class="page-width">
    <div class="testimonial-slider">
      <h2>
        Testimonials.
        <span class="color-gray"> Hear it straight from brands like yours</span>
      </h2>
      <p>Listen to what our customers have to say about us!</p>

      <client-only>
        <div class="flickity-controls">
          <img
            @click="previous1()"
            src="~/assets/icons/arrow-left.svg"
            alt="Slide Back"
            class="custom-arrow"
          />
          <img
            @click="next1()"
            src="~/assets/icons/arrow-right.svg"
            alt="Slide Next"
            class="custom-arrow"
          />
        </div>
        <VueSlickCarousel ref="carouselTesty" v-bind="slickOptions1">
          <div class="testimonial-slide">
            <img src="~/assets/images/citrix.svg" alt="Citrix Logo" />
            <p class="testi-text">
              Working with Travis was a great experience. He was on the ball and
              always got back to me quickly. On top of this, we received
              high-quality prints at a great price!
            </p>
            <div class="author-box">
              <div class="img">
                <img src="~/assets/images/author.webp" alt="Author Image" />
              </div>
              <div class="txt">
                <p class="name">BRAXTON ARD</p>
                <p class="location">United States</p>
              </div>
            </div>
          </div>
          <div class="testimonial-slide">
            <img src="~/assets/images/netflix.svg" alt="netflix Logo" />
            <p class="testi-text">
              Working with Travis was a great experience. He was on the ball and
              always got back to me quickly. On top of this, we received
              high-quality prints at a great price!
            </p>
            <div class="author-box">
              <div class="img">
                <img src="~/assets/images/author.webp" alt="Author Image" />
              </div>
              <div class="txt">
                <p class="name">BRAXTON ARD</p>
                <p class="location">United States</p>
              </div>
            </div>
          </div>
          <div class="testimonial-slide">
            <img src="~/assets/images/samsung.svg" alt="samsung Logo" />
            <p class="testi-text">
              Working with Travis was a great experience. He was on the ball and
              always got back to me quickly. On top of this, we received
              high-quality prints at a great price!
            </p>
            <div class="author-box">
              <div class="img">
                <img src="~/assets/images/author.webp" alt="Author Image" />
              </div>
              <div class="txt">
                <p class="name">BRAXTON ARD</p>
                <p class="location">United States</p>
              </div>
            </div>
          </div>
          <div class="testimonial-slide">
            <img src="~/assets/images/telogis.svg" alt="telogis Logo" />
            <p class="testi-text">
              Working with Travis was a great experience. He was on the ball and
              always got back to me quickly. On top of this, we received
              high-quality prints at a great price!
            </p>
            <div class="author-box">
              <div class="img">
                <img src="~/assets/images/author.webp" alt="Author Image" />
              </div>
              <div class="txt">
                <p class="name">BRAXTON ARD</p>
                <p class="location">United States</p>
              </div>
            </div>
          </div>
          <div class="testimonial-slide">
            <img src="~/assets/images/loews.svg" alt="loews Logo" />
            <p class="testi-text">
              Working with Travis was a great experience. He was on the ball and
              always got back to me quickly. On top of this, we received
              high-quality prints at a great price!
            </p>
            <div class="author-box">
              <div class="img">
                <img src="~/assets/images/author.webp" alt="Author Image" />
              </div>
              <div class="txt">
                <p class="name">BRAXTON ARD</p>
                <p class="location">United States</p>
              </div>
            </div>
          </div>
          <div class="testimonial-slide">
            <img src="~/assets/images/citrix.svg" alt="Citrix Logo" />
            <p class="testi-text">
              Working with Travis was a great experience. He was on the ball and
              always got back to me quickly. On top of this, we received
              high-quality prints at a great price!
            </p>
            <div class="author-box">
              <div class="img">
                <img src="~/assets/images/author.webp" alt="Author Image" />
              </div>
              <div class="txt">
                <p class="name">BRAXTON ARD</p>
                <p class="location">United States</p>
              </div>
            </div>
          </div>
        </VueSlickCarousel>
      </client-only>
    </div>
  </div>
</template>

<script>
export default {
  name: "TestimonialSlider",
  data() {
    return {
      slickOptions1: {
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
    next1() {
      this.$refs.carouselTesty.next();
    },

    previous1() {
      this.$refs.carouselTesty.prev();
    },
  },
};
</script>

<style lang="scss" scoped>
.testimonial-slider {
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
.testimonial-slide {
  height: 450px;
  border-radius: 20px;
  margin-right: 20px;
  display: flex !important;
  flex-direction: column;
  justify-content: space-between;
  gap: 30px;
  // width: 350px;
  padding: 30px;
  > img {
    width: 100%;
    height: 50px;
    object-fit: contain;
    object-position: left;
  }
  .testi-text {
    font-family: "BodyRegular";
    font-size: 18px;
    margin-top: 15px;
  }
  .author-box {
    display: flex;
    gap: 10px;
    img {
      width: 50px;
      height: 50px;
      object-fit: cover;
      border-radius: 50px;
    }
    .txt {
      display: flex;
      flex-direction: column;
      justify-content: center;
      p {
        margin: 0;
        font-size: 12px;
      }
      .name {
        font-family: "BodyMedium";
        font-size: 14px;
      }
    }
  }
}
.testimonial-slider .slick-slide:nth-child(1n) .testimonial-slide {
  background: #ffeae9;
}
.testimonial-slider .slick-slide:nth-child(2n) .testimonial-slide {
  background: #d9d2ff;
}
.testimonial-slider .slick-slide:nth-child(3n) .testimonial-slide {
  background: #fff3e9;
}
.testimonial-slider .slick-slide:nth-child(4n) .testimonial-slide {
  background: #e9f3ff;
}
.testimonial-slider .slick-slide:nth-child(5n) .testimonial-slide {
  background: #ebf2dd;
}
.testimonial-slider .slick-slide:nth-child(6n) .testimonial-slide {
  background: #ffeae9;
}
</style>