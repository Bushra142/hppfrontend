<template>
  <div class="page-width">
    <div class="faq-section">
      <h2>Frequently asked questions</h2>
      <p>Personalize your unboxing experience with a small surprise!</p>
      <div class="accordion faq-accordion" role="tablist">
        <b-card no-body class="single-faq">
          <a class="custom-toggle" v-b-toggle.faq-1
            >What is the purpose of carton packaging?</a
          >
          <b-collapse
            id="faq-1"
            visible
            accordion="my-accordion"
            role="tabpanel"
            class="custom-pane"
          >
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Optio,
            minus! Delectus amet obcaecati saepe. Laboriosam architecto ullam
            suscipit! Quos, molestiae! Placeat recusandae maxime maiores! At
            sapiente in corporis quaerat est.
          </b-collapse>
        </b-card>

        <b-card no-body class="single-faq">
          <a class="custom-toggle" v-b-toggle.faq-2
            >What is the purpose of carton packaging?</a
          >
          <b-collapse
            id="faq-2"
            accordion="my-accordion"
            role="tabpanel"
            class="custom-pane"
          >
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Optio,
            minus! Delectus amet obcaecati saepe. Laboriosam architecto ullam
            suscipit! Quos, molestiae! Placeat recusandae maxime maiores! At
            sapiente in corporis quaerat est.
          </b-collapse>
        </b-card>

        <b-card no-body class="single-faq">
          <a class="custom-toggle" v-b-toggle.faq-3
            >What is the purpose of carton packaging?</a
          >
          <b-collapse
            id="faq-3"
            accordion="my-accordion"
            role="tabpanel"
            class="custom-pane"
          >
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Optio,
            minus! Delectus amet obcaecati saepe. Laboriosam architecto ullam
            suscipit! Quos, molestiae! Placeat recusandae maxime maiores! At
            sapiente in corporis quaerat est.
          </b-collapse>
        </b-card>

        <b-card no-body class="single-faq">
          <a class="custom-toggle" v-b-toggle.faq-4
            >What is the purpose of carton packaging?</a
          >
          <b-collapse
            id="faq-4"
            accordion="my-accordion"
            role="tabpanel"
            class="custom-pane"
          >
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Optio,
            minus! Delectus amet obcaecati saepe. Laboriosam architecto ullam
            suscipit! Quos, molestiae! Placeat recusandae maxime maiores! At
            sapiente in corporis quaerat est.
          </b-collapse>
        </b-card>
      </div>

      <div class="ask-experts">
        <img src="~/assets/images/author.webp" />
        <p>
          Have other questions for us?
          <nuxt-link to="/">Ask our experts directly!</nuxt-link>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FaqSection",
  data() {
    return {
      myItems: [
        {
          title: "How many time zones are there in all?",
          value:
            "Given a 24-hour day and 360 degrees of longitude around the Earth",
        },
        {
          title: "How long is a day and year on Venus?",
          value:
            "Venus takes 224.7 Earth days to complete one orbit around the Sun.",
        },
        {
          title: "What animal smells like popcorn?",
          value: "Binturongs smell like popcorn.",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.faq-section {
  margin-top: 50px;
  margin-bottom: 50px;
  .ask-experts {
    background: #e7e3fd;
    border-radius: 10px;
    display: flex;
    align-items: center;
    gap: 30px;
    margin-top: 50px;
    img {
      width: 100px;
      margin-top: -20px;
      margin-bottom: -20px;
      margin-left: -20px;
    }
    p {
      margin: 0;
      a {
        color: black;
        text-decoration: none;
        border-bottom: 0.5px solid black;
      }
    }
  }
}
</style>