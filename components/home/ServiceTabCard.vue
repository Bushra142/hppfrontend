<template>
  <div class="tab-card">
    <img src="~/assets/icons/bulb.svg" alt="Service Icon" />
    <p>
      Get from idea to finished design quickly, with professionally made and
      editable templates.
    </p>
  </div>
</template>

<script>
export default {
  name: "ServiceTabcCard",
};
</script>

<style lang="scss" scoped>
.tab-card {
  border: 1px solid #707070;
  border-radius: 20px;
  padding: 20px;
  flex-basis: 23%;
  img {
    width: 30px;
    height: 30px;
    object-fit: contain;
  }
  p {
    font-size: 14px;
    margin: 0;
    margin-top: 15px;
  }
}
</style>