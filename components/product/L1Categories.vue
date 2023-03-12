<template>
  <div class="page-width">
    <div class="l-1-categories">
      <h2 class="mb-3">Categories</h2>
      <b-tabs pills card vertical lazy>
        <b-tab
          title="Vape and E-Cigarette Boxes"
          active
          @click="callApi('Category 1')"
        >
          <div v-if="loading" class="d-flex justify-content-center mb-3">
            <b-spinner label="Loading..."></b-spinner>
          </div>
          <l-1-category-card v-else />
        </b-tab>
        <b-tab
          title="Tobacco and Weed Packaging"
          @click="callApi('Category 2')"
        >
          <div v-if="loading" class="d-flex justify-content-center mb-3">
            <b-spinner label="Loading..."></b-spinner>
          </div>
          <l-1-category-card v-else />
        </b-tab>
        <b-tab
          title="CBD Skin Care Product Packaging"
          @click="callApi('Category 3')"
        >
          <div v-if="loading" class="d-flex justify-content-center mb-3">
            <b-spinner label="Loading..."></b-spinner>
          </div>
          <l-1-category-card v-else />
        </b-tab>
        <b-tab title="Cigarette Packaging" @click="callApi('Category 4')">
          <div v-if="loading" class="d-flex justify-content-center mb-3">
            <b-spinner label="Loading..."></b-spinner>
          </div>
          <l-1-category-card v-else />
        </b-tab>
        <b-tab title="Marijuana Packaging" @click="callApi('Category 5')">
          <div v-if="loading" class="d-flex justify-content-center mb-3">
            <b-spinner label="Loading..."></b-spinner>
          </div>
          <l-1-category-card v-else />
        </b-tab>
      </b-tabs>
    </div>
  </div>
</template>

<script>
import L1CategoryCard from "./L1CategoryCard.vue";
export default {
  components: { L1CategoryCard },
  name: "L1Categories",
  data() {
    return {
      loading: true,
    };
  },
  mounted() {
    this.loading = false;
  },
  methods: {
    callApi(categId) {
      this.loading = true;
      console.log(categId);
      setTimeout(() => {
        this.loading = false;
      }, 1500);
    },
  },
};
</script>

<style lang="scss" scoped>
.l-1-categories {
  margin-top: 50px;
  margin-bottom: 50px;
}
</style>