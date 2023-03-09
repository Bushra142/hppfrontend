<template>
  <header>
    <div class="top-bar-container">
      <div class="top-bar page-width">
        <div class="menu">
          <ul>
            <li><NuxtLink to="/tuck">Tuck Boxes</NuxtLink></li>
            <li><NuxtLink to="/tuck">Mailer Boxes</NuxtLink></li>
            <li><NuxtLink to="/tuck">CBD Boxes</NuxtLink></li>
            <li><NuxtLink to="/tuck">Cosmetic Boxes</NuxtLink></li>
          </ul>
        </div>
        <div class="cta">
          <a href="#!" class="cta-primary small"
            >Book a Call with Packaging Expert</a
          >
        </div>
      </div>
    </div>
    <div class="logo-bar page-width">
      <div class="logo">
        <HPPLogo />
        <search />
      </div>
      <div class="contacts">
        <a href="tel: 866-225-2112" class="color-primary text-semi">
          866-225-2112
        </a>
        |
        <a
          href="mailto:orders@halfpricepackaging.com"
          class="color-primary text-semi"
          >orders@halfpricepackaging.com</a
        >
      </div>
    </div>
    <div class="menu-bar page-width">
      <div class="menu">
        <ul class="nav-custom">
          <li class="nav-link-c">Industries</li>
          <li class="nav-link-c">Shapes & Style</li>
          <li class="nav-link-c">
            <NuxtLink to="/material">Material</NuxtLink>
          </li>
          <li class="nav-link-c">
            <NuxtLink to="/portfolio">Portfolio</NuxtLink>
          </li>
          <li class="nav-link-c"><NuxtLink to="/blog">Insights</NuxtLink></li>
          <li class="nav-link-c">
            <NuxtLink to="/finishes">Premium Finishes</NuxtLink>
          </li>
          <li class="nav-link-c">
            <NuxtLink to="/about">About</NuxtLink>
          </li>
        </ul>
      </div>
      <div class="icons">
        <a href="#!" class="social-icon"><img src="~/assets/icons/fb.svg" /></a>
        <a href="#!" class="social-icon"><img src="~/assets/icons/tw.svg" /></a>
        <a href="#!" class="social-icon"><img src="~/assets/icons/ig.svg" /></a>
        <a href="#!" class="social-icon"><img src="~/assets/icons/ln.svg" /></a>
        <a href="#!" class="social-icon"><img src="~/assets/icons/yt.svg" /></a>

        <a href="#!" class="cta-primary outlined small">Get a Quote</a>
      </div>
    </div>
  </header>
</template>

<script>
import Search from "./Search.vue";
export default {
  components: { Search },
  name: "HeaderMain",
};
</script>

<style lang="scss" scoped>
.top-bar-container {
  background: #eeeeee;
  padding-top: 8px;
  padding-bottom: 8px;
  font-size: 14px;
  .top-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    .menu {
      ul {
        display: flex;
        list-style: none;
        gap: 20px;
        a:hover {
          text-decoration: none;
          color: #7157f8;
        }
      }
    }
  }
}

.logo-bar {
  padding-top: 15px;
  padding-bottom: 15px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  .logo {
    display: flex;
    align-items: center;
    gap: 40px;
  }
  .contacts {
    display: flex;
    gap: 10px;
  }
}

.menu-bar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-top: 15px;
  padding-bottom: 15px;
  .menu {
    .nav-custom {
      display: flex;
      list-style: none;
      gap: 20px;
      .nav-link-c {
        a:hover {
          text-decoration: none;
          color: #7157f8;
        }
      }
    }
  }
  .icons {
    display: flex;
    align-items: center;
    gap: 20px;
    .social-icon {
      filter: grayscale(1);
      img {
        height: 20px;
      }
      &:hover {
        filter: none;
      }
    }
  }
}
</style>