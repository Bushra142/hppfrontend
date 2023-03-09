<template>
  <div>
    <hero />
    <questions-form />
    <usp-bar />
    <industry-slider />
    <featured-industries />
    <usp-reviews />
    <two-step-form />
    <service-tabs />
    <video-sect />
    <testimonial-slider />
    <people-cards />
    <faq-section />
    <insta-slider />
    <contact-us-questions />
  </div>
</template>

<script>
import FeaturedIndustries from "../components/home/FeaturedIndustries.vue";
import Hero from "../components/home/Hero.vue";
import IndustrySlider from "../components/home/IndustrySlider.vue";
import PeopleCards from "../components/PeopleCards.vue";
import QuestionsForm from "../components/home/QuestionsForm.vue";
import ServiceTabs from "../components/home/ServiceTabs.vue";
import TestimonialSlider from "../components/TestimonialSlider.vue";
import TwoStepForm from "../components/home/TwoStepForm.vue";
import UspBar from "../components/home/UspBar.vue";
import UspReviews from "../components/home/UspReviews.vue";
import VideoSect from "../components/home/VideoSect.vue";
import FaqSection from "../components/FaqSection.vue";
import InstaSlider from "../components/InstaSlider.vue";
import ContactUsQuestions from "../components/ContactUsQuestions.vue";
export default {
  components: {
    Hero,
    QuestionsForm,
    UspBar,
    IndustrySlider,
    FeaturedIndustries,
    UspReviews,
    TwoStepForm,
    ServiceTabs,
    VideoSect,
    TestimonialSlider,
    PeopleCards,
    FaqSection,
    InstaSlider,
    ContactUsQuestions,
  },
  name: "IndexPage",
  head() {
    return {
      title: "Custom Boxes With Logo | Custom Printing and Packaging Wholesale",
    };
  },
};
</script>
