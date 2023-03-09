<template>
  <div class="page-width">
    <div class="testimonial-slider">
      <h2>
        Testimonials.
        <span class="color-gray"> Hear it straight from brands like yours</span>
      </h2>
      <p>Listen to what our customers have to say about us!</p>
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
          <div class="carousel-cell testimonial-slide">
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
          <div class="carousel-cell testimonial-slide">
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
          <div class="carousel-cell testimonial-slide">
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
          <div class="carousel-cell testimonial-slide">
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
          <div class="carousel-cell testimonial-slide">
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
          <div class="carousel-cell testimonial-slide">
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
        </flickity>
      </client-only>
    </div>
  </div>
</template>

<script>
export default {
  name: "TestimonialSlider",
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
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 30px;
  width: 350px;
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
.testimonial-slide:nth-child(1) {
  background: #ffeae9;
}
.testimonial-slide:nth-child(2) {
  background: #d9d2ff;
}
.testimonial-slide:nth-child(3) {
  background: #fff3e9;
}
.testimonial-slide:nth-child(4) {
  background: #e9f3ff;
}
.testimonial-slide:nth-child(5) {
  background: #ebf2dd;
}
.testimonial-slide:nth-child(6) {
  background: #ffeae9;
}
</style>