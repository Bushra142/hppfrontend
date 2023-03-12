<template>
  <div>
    <l-one-header />
    <usp-bar />
    <category-slider />
    <l-1-categories />
    <zig-zag-left />
    <zig-zag-right />
    <testimonial-slider />
    <people-cards />
    <faq-section />
    <insta-slider />
    <contact-us-questions />
  </div>
</template>

<script>
import TestimonialSlider from "../../components/TestimonialSlider.vue";
import PeopleCards from "../../components/PeopleCards.vue";
import FaqSection from "../../components/FaqSection.vue";
import InstaSlider from "../../components/InstaSlider.vue";
import ContactUsQuestions from "../../components/ContactUsQuestions.vue";
import LOneHeader from "../../components/product/LOneHeader.vue";
import UspBar from "../../components/home/UspBar.vue";
import CategorySlider from "../../components/product/CategorySlider.vue";
import L1Categories from "../../components/product/L1Categories.vue";
import ZigZagLeft from "../../components/product/ZigZagLeft.vue";
import ZigZagRight from "../../components/product/ZigZagRight.vue";
export default {
  components: {
    TestimonialSlider,
    PeopleCards,
    FaqSection,
    InstaSlider,
    ContactUsQuestions,
    LOneHeader,
    UspBar,
    CategorySlider,
    L1Categories,
    ZigZagLeft,
    ZigZagRight,
  },
  name: "ProductL2",
};
</script>

<style lang="scss" scoped>
</style>