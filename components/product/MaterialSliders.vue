<template>
  <div class="page-width usp-sliders">
    <div class="shipping usp-row">
      <div class="text-area">
        <h2 class="color-primary">
          <img src="~/assets/icons/shipping.svg" alt="Shipping Icon" />
          Shipping
        </h2>
        <p>
          Give your packages a branded and personalized touch with custom Tissue
          Paper. With low minimums, you can switch up your noissue Tissue for
          seasonal collections
        </p>
      </div>
      <div class="slider-area">
        <client-only>
          <VueSlickCarousel
            :slidesToShow="4"
            :adaptiveHeight="true"
            :focusOnSelect="true"
            class="materialSlider"
          >
            <div class="material-slide">
              <img src="~/assets/images/s1.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s2.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s3.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s4.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s5.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s6.png" alt="Hello" draggable="false" />
            </div>
          </VueSlickCarousel>
        </client-only>
      </div>
    </div>
    <div class="shipping usp-row">
      <div class="text-area">
        <h2 class="color-primary">
          <img src="~/assets/icons/material.svg" alt="Material Icon" />
          Material
        </h2>
        <p>
          Give your packages a branded and personalized touch with custom Tissue
          Paper. With low minimums, you can switch up your noissue Tissue for
          seasonal collections
        </p>
      </div>
      <div class="slider-area">
        <client-only>
          <VueSlickCarousel
            :slidesToShow="4"
            :adaptiveHeight="true"
            :focusOnSelect="true"
            class="materialSlider"
          >
            <div class="material-slide">
              <img src="~/assets/images/s1.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s2.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s3.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s4.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s5.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s6.png" alt="Hello" draggable="false" />
            </div>
          </VueSlickCarousel>
        </client-only>
      </div>
    </div>
    <div class="shipping usp-row">
      <div class="text-area">
        <h2 class="color-primary">
          <img src="~/assets/icons/adons.svg" alt="Ads-Ons & Finishing Icon" />
          Ad-Ons & Finishing
        </h2>
        <p>
          Give your packages a branded and personalized touch with custom Tissue
          Paper. With low minimums, you can switch up your noissue Tissue for
          seasonal collections
        </p>
      </div>
      <div class="slider-area">
        <client-only>
          <VueSlickCarousel
            :slidesToShow="4"
            :adaptiveHeight="true"
            :focusOnSelect="true"
            class="materialSlider"
          >
            <div class="material-slide">
              <img src="~/assets/images/s1.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s2.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s3.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s4.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s5.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s6.png" alt="Hello" draggable="false" />
            </div>
          </VueSlickCarousel>
        </client-only>
      </div>
    </div>
    <div class="shipping usp-row">
      <div class="text-area">
        <h2 class="color-primary">
          <img src="~/assets/icons/paper.svg" alt="Paper Weight Icon" />
          Paper Weight
        </h2>
        <p>
          Give your packages a branded and personalized touch with custom Tissue
          Paper. With low minimums, you can switch up your noissue Tissue for
          seasonal collections
        </p>
      </div>
      <div class="slider-area">
        <client-only>
          <VueSlickCarousel
            :slidesToShow="4"
            :adaptiveHeight="true"
            :focusOnSelect="true"
            class="materialSlider"
          >
            <div class="material-slide">
              <img src="~/assets/images/s1.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s2.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s3.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s4.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s5.png" alt="Hello" draggable="false" />
            </div>
            <div class="material-slide">
              <img src="~/assets/images/s6.png" alt="Hello" draggable="false" />
            </div>
          </VueSlickCarousel>
        </client-only>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MaterialSliders",
};
</script>

<style lang="scss" scoped>
.usp-sliders {
  .usp-row {
    display: flex;
    border-bottom: 1px solid #707070;
    .text-area {
      flex-basis: 50%;
      padding: 50px;
      padding-left: 0;
      h2 {
        img {
          width: 40px;
          margin-right: 40px;
        }
        margin-bottom: 20px;
      }
      p {
        font-size: 16px;
      }
    }
    .slider-area {
      flex-basis: 50%;
      overflow: hidden;
      padding: 50px;
    }
  }
  .usp-row:nth-last-child(1) {
    border: none;
  }
}
.material-slide {
  padding: 10px;
  img {
    border-radius: 10px;
    // width: 80px;
    height: 120px;
    width: 100%;
    object-fit: cover;
  }
}
</style>