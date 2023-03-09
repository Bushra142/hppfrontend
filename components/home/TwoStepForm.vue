<template>
  <div class="page-width">
    <div class="two-step-form">
      <h2>
        Have questions?
        <span class="color-gray">We have answers</span>
      </h2>
      <p>
        Fill out the form and your dedicated packaging consultant will get in
        touch!
      </p>
      <div class="usps">
        <b-card no-body>
          <b-tabs pills card v-model="tabIndex">
            <b-tab title="1. Project Info" active
              ><b-card-text>
                <div class="text-right">
                  <a href="#!" @click="tabIndex++" class="cta-primary  m-3"
                    >Proceed</a
                  >
                </div>
              </b-card-text></b-tab
            >
            <b-tab title="2. Contact Info"
              ><b-card-text>aaaaa</b-card-text
            ></b-tab>
          </b-tabs>
        </b-card>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TwoStepForm",
  data() {
    return {
      tabIndex: 0,
    };
  },
};
</script>

<style lang="scss" scoped>
.two-step-form {
  background: #f3f3f3;
  padding: 50px;
  border-radius: 20px;
}
</style>