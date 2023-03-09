<template>
  <div class="page-width">
    <div class="usp-reviews">
      <h2>
        Delivering total packaging
        <br />
        <span class="color-gray">success with real results</span>
      </h2>
      <p>Grow your business with eco-friendly alternatives to packaging.</p>
      <div class="usps">
        <b-card no-body>
          <b-tabs pills card>
            <b-tab title="Cost Saving" active
              ><b-card-text><review-1 /></b-card-text
            ></b-tab>
            <b-tab title="Time Saving"
              ><b-card-text><review-2 /></b-card-text
            ></b-tab>
            <b-tab title="Reliability"
              ><b-card-text><review-3 /></b-card-text
            ></b-tab>
            <b-tab title="Brand Impact"
              ><b-card-text><review-4 /></b-card-text
            ></b-tab>
            <b-tab title="Sustainability"
              ><b-card-text><review-5 /></b-card-text
            ></b-tab>
          </b-tabs>
        </b-card>
      </div>
    </div>
  </div>
</template>

<script>
import Review1 from "../reviews/Review1.vue";
import Review2 from "../reviews/Review2.vue";
import Review3 from "../reviews/Review3.vue";
import Review4 from "../reviews/Review4.vue";
import Review5 from "../reviews/Review5.vue";
export default {
  components: { Review1, Review2, Review3, Review4, Review5 },
  name: "UspReviews",
};
</script>

<style lang="scss" scoped>
.usp-reviews {
  margin-top: 50px;
  margin-bottom: 50px;
  .usps {
    padding-top: 30px;
  }
}
</style>