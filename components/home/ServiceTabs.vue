<template>
  <div class="page-width">
    <div class="service-tabs">
      <div class="entry">
        <h2>
          Services that
          <span class="color-gray">meet your packaging needs</span>
        </h2>
        <p>
          Our 360 PakFactory approach delivers all the services you need to
          create the best packaging solutions your products and business needs
          in order to acheive total packaging success.
        </p>
      </div>
      <div class="usps services">
        <b-tabs content-class="mt-3">
          <b-tab title="Consultation" active>
            <service-tab-card />
            <service-tab-card />
            <service-tab-card />
            <service-tab-card />
          </b-tab>
          <b-tab title="Design">
            <service-tab-card />
            <service-tab-card
          /></b-tab>
          <b-tab title="Prototype">
            <service-tab-card /> <service-tab-card /> <service-tab-card />
          </b-tab>
        </b-tabs>
      </div>
    </div>
  </div>
</template>

<script>
import ServiceTabCard from "./ServiceTabCard.vue";
export default {
  components: {
    ServiceTabCard,
  },
  name: "ServiceTabs",
};
</script>

<style lang="scss" scoped>
.service-tabs {
  margin-top: 50px;
  margin-bottom: 50px;
  .entry {
    width: 65%;
  }
  .services {
  }
}
</style>