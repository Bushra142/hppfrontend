<template>
  <div class="page-width">
    <div class="usp-bar">
      <div class="review-logos">
        <img src="~/assets/images/reviews.webp" alt="HPP Reviews" />
      </div>
      <div class="usps">
        <div class="usp">
          <img src="~/assets/icons/fast-time.svg" alt="Quick Turnaround icon" />
          <p>Quick Turnaround</p>
        </div>
        <div class="usp">
          <img src="~/assets/icons/delivery.svg" alt="Fast delivery icon" />
          <p>Super-Fast Delivery</p>
        </div>
        <div class="usp">
          <img src="~/assets/icons/3d.svg" alt="3d Design studio icon" />
          <p>3D Design Studio</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "UspBar",
};
</script>

<style lang="scss" scoped>
.usp-bar {
  background: #e1dbff;
  padding: 20px 50px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  border-radius: 10px;
  .review-logos {
    img {
      max-width: 400px;
    }
  }
  .usps {
    display: flex;
    align-items: center;
    gap: 30px;
    .usp {
      display: flex;
      align-items: center;
      gap: 10px;
      img {
        width: 35px;
        height: 35px;
        object-fit: contain;
      }
      p {
        font-size: 14px;
        margin: 0;
      }
    }
  }
}
</style>