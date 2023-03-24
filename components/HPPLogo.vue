<template>
  <nuxt-link to="/">
    <img src="/logo.svg" alt="Half Price Packaging Logo" class="hpp-logo"
  /></nuxt-link>
</template>

<script>
export default {
  name: "HppLogo",
};
</script>


<style>
.hpp-logo {
  width: 250px;
}
@media (max-width: 480px) {
  .hpp-logo {
    width: 160px;
  }
}
</style>
