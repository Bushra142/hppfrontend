<template>
  <div class="product-specs">
    <div class="page-width">
      <h2>Product Specification</h2>
      <div class="specs-table">
        <div class="spec-row">
          <div class="spec-heading">Box Style</div>
          <div class="spec-text">Hemp Boxes</div>
        </div>
        <div class="spec-row">
          <div class="spec-heading">Dimension (L + W + H)</div>
          <div class="spec-text">All Custom Sizes & Shapes</div>
        </div>
        <div class="spec-row">
          <div class="spec-heading">Quantities</div>
          <div class="spec-text">No Minimum Order Required</div>
        </div>
        <div class="spec-row">
          <div class="spec-heading">Paper Stock</div>
          <div class="spec-text">
            10pt to 28pt (60lb to 400lb) Eco-Friendly Kraft, E-flute Corrugated,
            Bux Board, Cardstock
          </div>
        </div>
        <div class="spec-row">
          <div class="spec-heading">Printing</div>
          <div class="spec-text">
            No Printing, CMYK, CMYK + 1 PMS color, CMYK + 2 PMS colors
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductSpecification",
};
</script>

<style lang="scss" scoped>
.product-specs {
  background: #dfdafb;
  padding-top: 50px;
  padding-bottom: 50px;
  margin-top: 50px;
  margin-bottom: 50px;  
  .specs-table {
    margin-top: 30px;
    .spec-row {
      display: flex;
      font-size: 18px;
      .spec-heading {
        flex-basis: 40%;
        border-right: 3px solid #7157f8;
        font-family: "BodyMedium";
        padding: 15px 0;
      }
      .spec-text {
        flex-basis: 50%;
        padding: 15px 0;
        padding-left: 30px;
      }
    }
  }
}
</style>