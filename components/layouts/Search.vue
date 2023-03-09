<template>
  <div>
    <div class="search-container">
      <input
        type="search"
        id="hppsearch"
        name="hppsearch"
        placeholder="Search Category"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: "Search",
};
</script>

<style lang="scss" scoped>
#hppsearch {
  all: unset;
  min-width: 350px;
  padding: 10px 20px;
  padding-right: 45px;
  background: url("/search.svg") no-repeat right, #f2f2f2;
  background-size: 20px;
  background-position: 96%;
}

@media (max-width: 640px) {
  #hppsearch {
    min-width: 100%;
  }
}
</style>