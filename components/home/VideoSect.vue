<template>
  <div class="page-width">
    <div class="video-sect">
      <div class="entry text-center">
        <!-- <iframe
          style="aspect-ratio: 16/9; width: 80%"
          src="https://www.youtube.com/embed/GmDOvGXpUTA"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen=""
        ></iframe> -->
        <h2>Total packaging success with 360° half price packaging approach</h2>
      </div>
      <div class="unique-usps">
        <div class="usp">
          <img
            src="~/assets/icons/global-search.svg"
            alt="Global sourcing icon"
          />
          <h4>Global Sourcing</h4>
          <p>
            Get from idea to finished design quickly, with professionally made
            and editable templates.
          </p>
        </div>
        <div class="usp">
          <img
            src="~/assets/icons/global-search.svg"
            alt="Global sourcing icon"
          />
          <h4>Price Matching</h4>
          <p>
            Get from idea to finished design quickly, with professionally made
            and editable templates.
          </p>
        </div>
        <div class="usp">
          <img
            src="~/assets/icons/global-search.svg"
            alt="Global sourcing icon"
          />
          <h4>HPP as sourcing Partner</h4>
          <p>
            Get from idea to finished design quickly, with professionally made
            and editable templates.
          </p>
        </div>
        <div class="usp">
          <img
            src="~/assets/icons/global-search.svg"
            alt="Global sourcing icon"
          />
          <h4>Contract Packaging</h4>
          <p>
            Get from idea to finished design quickly, with professionally made
            and editable templates.
          </p>
        </div>
        <div class="usp">
          <img
            src="~/assets/icons/global-search.svg"
            alt="Global sourcing icon"
          />
          <h4>Warehousing and IMS</h4>
          <p>
            Get from idea to finished design quickly, with professionally made
            and editable templates.
          </p>
        </div>
        <div class="usp">
          <img
            src="~/assets/icons/global-search.svg"
            alt="Global sourcing icon"
          />
          <h4>3PL service</h4>
          <p>
            Get from idea to finished design quickly, with professionally made
            and editable templates.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VideoSect",
};
</script>

<style lang="scss" scoped>
.video-sect {
  background: #ebf2dd;
  padding: 50px;
  border-radius: 20px;
  .entry {
    h2 {
      width: 50%;
      margin: 30px auto;
    }
    margin-bottom: 50px;
  }
  .unique-usps {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    .usp {
      flex-basis: 32%;
      img {
        width: 30px;
        height: 30px;
        object-fit: contain;
      }
      h4 {
        font-size: 18px;
        margin-top: 15px;
      }
      p {
        font-size: 18px;
      }
    }
  }
}
</style>