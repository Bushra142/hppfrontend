<template>
  <div>
    <!-- Send category data here by props -->
    <div class="l-1-category-card">
      <div class="categ-cards">
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat1.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat2.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat3.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat1.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat2.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat3.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat1.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat2.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat3.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat1.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat2.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
        <div class="categ-card">
          <nuxt-link to="/l2">
            <img src="~/assets/images/cat3.png" alt="Image src" />
            <h4>Custom Multi Colored Tissue Paper</h4>
          </nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "L1CategoryCard",
};
</script>

<style lang="scss" scoped>
.l-1-category-card {
  .categ-cards {
    display: flex;
    flex-wrap: wrap;
    .categ-card {
      flex-basis: 33.3%;
      padding: 10px;
      padding-top: 0;
      padding-bottom: 20px;
      a {
        color: inherit;
        text-decoration: none;
        text-align: center;
      }
      img {
        width: 100%;
        height: 220px;
        object-fit: cover;
        border-radius: 20px;
      }
      h4 {
        font-size: 18px;
        margin-top: 15px;
      }
    }
  }
}
</style>