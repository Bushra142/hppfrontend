<template>
  <div>
    <header-main />
    <Nuxt />
    <footer-main />
  </div>
</template>

<script>
import FooterMain from "../components/layouts/Footer.vue";
import HeaderMain from "../components/layouts/Header.vue";
export default {
  components: {
    HeaderMain,
    FooterMain,
  },
};
</script>

<style lang="scss" scoped>
</style>