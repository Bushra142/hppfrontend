<template>
  <footer class="page-width">
    <div class="footer-top">
      <div class="entry"></div>
      <div class="two-parts">
        <div class="logo-part">
          <h2>
            You've just found your last
            <br />
            <span class="color-gray"> packaging partner</span>
          </h2>
          <div class="logos">
            <img src="~/assets/images/iso.svg" alt="Iso certification logo" />
          </div>
          <p>
            Your brand deserves a credit for doing the right thing! Share the
            good news and join our eco-alliance.
          </p>
        </div>
        <div class="menu-part">
          <div class="contact-box">
            <h4>Quick Links</h4>
            <ul class="footer-menu">
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
            </ul>
          </div>
          <div class="contact-box">
            <h4>Contact</h4>
            <a href="tel:866-225-2112">866-225-2112</a>
            <a href="mailto:orders@halfpricepackaging.com"
              >orders@halfpricepackaging.com</a
            >
            <a href="mailto:sales@halfpricepackaging.com"
              >sales@halfpricepackaging.com</a
            >
          </div>
          <div class="contact-box">
            <h4>Quick Links</h4>
            <ul class="footer-menu">
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
            </ul>
          </div>
          <div class="contact-box">
            <h4>Quick Links</h4>
            <ul class="footer-menu">
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
              <li><nuxt-link to="'/'">Rigid Boxes</nuxt-link></li>
            </ul>
          </div>
        </div>
      </div>
      <div class="exit">
        <p class="color-primary">
          © 2022 Half Price Packaging. All Rights Reserved.
        </p>
        <div class="icons">
          <a href="#!" class="social-icon"
            ><img src="~/assets/icons/fb.svg"
          /></a>
          <a href="#!" class="social-icon"
            ><img src="~/assets/icons/tw.svg"
          /></a>
          <a href="#!" class="social-icon"
            ><img src="~/assets/icons/ig.svg"
          /></a>
          <a href="#!" class="social-icon"
            ><img src="~/assets/icons/ln.svg"
          /></a>
          <a href="#!" class="social-icon"
            ><img src="~/assets/icons/yt.svg"
          /></a>

          <a href="#!" class="trust-pilot"
            ><img src="~/assets/images/trustpilot.svg" alt="Trustpilot logo"
          /></a>
        </div>
      </div>
    </div>
    <div class="footer-bottom"></div>
  </footer>
</template>

<script>
export default {
  name: "FooterMain",
};
</script>

<style lang="scss" scoped>
.footer-top {
  margin-top: 50px;
  margin-bottom: 20px;
  background: #f2f2f2;
  border-radius: 30px;
  padding: 50px;
  padding-bottom: 20px;
  .entry {
  }
  .two-parts {
    display: flex;
    .logo-part {
      flex-basis: 50%;
      .logos {
        margin-top: 40px;
        margin-bottom: 25px;
        img {
          width: 220px;
        }
      }
    }
    .menu-part {
      flex-basis: 50%;
      display: flex;
      flex-wrap: wrap;
      .contact-box {
        flex-basis: 50%;
        padding: 20px;
        padding-top: 0;
        margin-bottom: 20px;
        > a {
          text-decoration: none;
          color: black;
          margin-bottom: 5px;
          display: block;
        }
        .footer-menu {
          li {
            margin-bottom: 5px;
            a {
              text-decoration: none;
              color: black;
            }
          }
        }
      }
    }
  }
  .exit {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border-top: 1px solid #707070;
    padding-top: 20px;
    p {
      font-size: 14px;
      margin: 0;
    }
    .icons {
      display: flex;
      align-items: center;
      gap: 30px;
      .social-icon {
        filter: brightness(0);
        img {
          height: 18px;
        }
      }
      .trust-pilot {
        img {
          width: 120px;
        }
      }
    }
  }
}

.footer-bottom {
}
</style>