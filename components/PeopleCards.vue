<template>
  <div class="page-width">
    <div class="people-cards">
      <div class="entry">
        <h2>
          People.
          <span class="color-gray">
            Putting the help in Half Price packaging</span
          >
        </h2>
        <p>Grow your business with eco-friendly alternatives to packaging.</p>
      </div>
      <div class="cards">
        <div class="full-card">
          <p>
            Out expert team is on hand to help you unlock branded packaging that
            does no harm to the planet.
          </p>
          <a href="#!" class="cta-primary small mt-3">Say Hello!</a>
        </div>
        <div class="half-card">
          <nuxt-link to="/" class="p-card">
            <p>
              Dedicated account managers who help you from start to finish and
              beyond.
            </p>
            <img src="~/assets/icons/open-box.svg" alt="Open Box Icon" />
          </nuxt-link>
          <nuxt-link to="/" class="p-card">
            <p>Find a better price and we’ll beat it by up to 20%.</p>
            <img src="~/assets/icons/mail.svg" alt="Mail Icon" />
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "PeopleCards",
};
</script>

<style lang="scss" scoped>
.people-cards {
  margin-top: 50px;
  margin-bottom: 50px;
  .entry {
  }
  .cards {
    display: flex;
    gap: 25px;
    .full-card {
      flex-basis: 50%;
      border-radius: 20px;
      padding: 30px;
      background: url(/_nuxt/assets/images/hellobg.webp), #f2f2f2;
      background-size: 450px;
      background-repeat: no-repeat;
      background-position: bottom;
      background-position-y: 80%;
    }
    .half-card {
      flex-basis: 50%;
      display: flex;
      flex-direction: column;
      gap: 25px;
      .p-card {
        text-decoration: none;
        color: inherit;
        background: #f2f2f2;
        border-radius: 20px;
        padding: 30px;
        text-align: right;
        p {
          text-align: left;
        }
        img {
          width: 90px;
        }
      }
    }
  }
}
</style>