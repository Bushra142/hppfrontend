<template>
  <div class="page-width">
    <div class="featured-industries">
      <div class="entry">
        <div class="headline">
          <h2>
            One for all solution,
            <span class="color-gray">for custom printed packaging</span>
          </h2>
          <p>
            Get everything custom packaging your business needs all in one
            place.
          </p>
        </div>
        <div class="cta">
          <a href="#!" class="cta-primary outlined">Browse all catalog</a>
        </div>
      </div>
      <div class="industry-cards">
        <div class="industry-card">
          <nuxt-link to="/">
            <img src="~/assets/images/card.webp" alt="Card" />
            <h4 class="slide-title">Folding Carton Boxes</h4>
            <p>Standard cardstock boxes made from thin, flexible paperboard</p>
          </nuxt-link>
        </div>
        <div class="industry-card">
          <nuxt-link to="/">
            <img src="~/assets/images/card.webp" alt="Card" />
            <h4 class="slide-title">Folding Carton Boxes</h4>
            <p>Standard cardstock boxes made from thin, flexible paperboard</p>
          </nuxt-link>
        </div>
        <div class="industry-card">
          <nuxt-link to="/">
            <img src="~/assets/images/card.webp" alt="Card" />
            <h4 class="slide-title">Folding Carton Boxes</h4>
            <p>Standard cardstock boxes made from thin, flexible paperboard</p>
          </nuxt-link>
        </div>
        <div class="industry-card">
          <nuxt-link to="/">
            <img src="~/assets/images/card.webp" alt="Card" />
            <h4 class="slide-title">Folding Carton Boxes</h4>
            <p>Standard cardstock boxes made from thin, flexible paperboard</p>
          </nuxt-link>
        </div>
        <div class="industry-card">
          <nuxt-link to="/">
            <img src="~/assets/images/card.webp" alt="Card" />
            <h4 class="slide-title">Folding Carton Boxes</h4>
            <p>Standard cardstock boxes made from thin, flexible paperboard</p>
          </nuxt-link>
        </div>
        <div class="industry-card">
          <nuxt-link to="/">
            <img src="~/assets/images/card.webp" alt="Card" />
            <h4 class="slide-title">Folding Carton Boxes</h4>
            <p>Standard cardstock boxes made from thin, flexible paperboard</p>
          </nuxt-link>
        </div>
        <div class="industry-card">
          <nuxt-link to="/">
            <img src="~/assets/images/card.webp" alt="Card" />
            <h4 class="slide-title">Folding Carton Boxes</h4>
            <p>Standard cardstock boxes made from thin, flexible paperboard</p>
          </nuxt-link>
        </div>
        <div class="industry-card">
          <nuxt-link to="/">
            <img src="~/assets/images/card.webp" alt="Card" />
            <h4 class="slide-title">Looking for something eles?</h4>
            <p>Standard cardstock boxes made from thin, flexible paperboard</p>
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FeaturedIndustries",
};
</script>

<style lang="scss" scoped>
.featured-industries {
  .entry {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 30px;
    .headline {
    }
    .cta {
    }
  }
  .industry-cards {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    justify-content: space-between;
    .industry-card {
      flex-basis: 23%;
      a {
        color: inherit;
        text-decoration: none;
      }
      img {
        border-radius: 30px;
        width: 100%;
        transition: 0.2s ease-in all;
        &:hover {
          filter: drop-shadow(6px 6px 12px rgba(0, 0, 0, 0.12));
        }
      }
      h4 {
        font-size: 18px;
        margin-top: 15px;
      }
      p {
        font-size: 14px;
      }
    }
  }
}
</style>