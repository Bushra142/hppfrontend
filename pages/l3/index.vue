<template>
  <div>
    <l-three-header />
    <usp-bar />
    <product-specification />
    <gallery-carousel />
    <product-description />
    <classic-styles />
    <zig-zag-left />
    <zig-zag-right />
    <material-sliders />
    <zig-zag-left />
    <zig-zag-right />
    
    <faq-section />
    <insta-slider />
    <contact-us-questions />
  </div>
</template>

<script>
import FaqSection from "../../components/FaqSection.vue";
import InstaSlider from "../../components/InstaSlider.vue";
import ContactUsQuestions from "../../components/ContactUsQuestions.vue";
import LThreeHeader from "../../components/product/LThreeHeader.vue";
import UspBar from "../../components/home/UspBar.vue";
import ZigZagLeft from "../../components/product/ZigZagLeft.vue";
import ZigZagRight from "../../components/product/ZigZagRight.vue";
import ProductSpecification from "../../components/product/ProductSpecification.vue";
import GalleryCarousel from "../../components/product/GalleryCarousel.vue";
import ProductDescription from "../../components/product/ProductDescription.vue";
import ClassicStyles from "../../components/product/ClassicStyles.vue";
import MaterialSliders from "../../components/product/MaterialSliders.vue";
export default {
  components: {
    FaqSection,
    InstaSlider,
    ContactUsQuestions,
    LThreeHeader,
    UspBar,
    ZigZagLeft,
    ZigZagRight,
    ProductSpecification,
    GalleryCarousel,
    ProductDescription,
    ClassicStyles,
    MaterialSliders,
  },
  name: "ProductL3",
};
</script>

<style lang="scss" scoped>
</style>