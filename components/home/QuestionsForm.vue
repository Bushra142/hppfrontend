<template>
  <div class="page-width questions-form">
    <h2 v-b-toggle.questions-form class="arrow-bg">
      Have questions?
      <span class="color-gray">We have answers</span>
    </h2>
    <p>
      Fill out the form and your dedicated packaging consultant will get in
      touch!
    </p>

    <b-collapse id="questions-form" class="mt-2">
      <b-card>
        <p class="card-text">Collapse contents Here</p>
      </b-card>
    </b-collapse>
  </div>
</template>

<script>
export default {
  name: "QuestionsForm",
};
</script>

<style lang="scss" scoped>
.questions-form {
  margin-top: 50px;
  margin-bottom: 50px;
  .arrow-bg {
    position: relative;
  }
  .arrow-bg::before {
    content: url("~/assets/icons/arrow-down.svg");
    font-size: 1.2em;
    position: absolute;
    top: 3px;
    right: 0em;
    transition: 0.2s ease-in all;
  }
  .arrow-bg.not-collapsed::before {
    transform: rotate(180deg);
  }
}
</style>