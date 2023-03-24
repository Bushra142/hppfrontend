<template>
  <header>
    <div class="desktop-header">
      <div class="top-bar-container">
        <div class="top-bar page-width">
          <div class="menu">
            <ul>
              <li><nuxt-link to="'/tuck'">Tuck Boxes</nuxt-link></li>
              <li><nuxt-link to="'/tuck'">Mailer Boxes</nuxt-link></li>
              <li><nuxt-link to="'/tuck'">CBD Boxes</nuxt-link></li>
              <li><nuxt-link to="'/tuck'">Cosmetic Boxes</nuxt-link></li>
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
          <hpp-logo />
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
              <nuxt-link to="'/material'">Material</nuxt-link>
            </li>
            <li class="nav-link-c">
              <nuxt-link to="'/portfolio'">Portfolio</nuxt-link>
            </li>
            <li class="nav-link-c"><NuxtLink to="/blog">Insights</NuxtLink></li>
            <li class="nav-link-c">
              <nuxt-link to="'/finishes'">Premium Finishes</nuxt-link>
            </li>
            <li class="nav-link-c">
              <nuxt-link to="'/about'">About</nuxt-link>
            </li>
          </ul>
        </div>
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

          <a href="#!" class="cta-primary outlined small">Get a Quote</a>
        </div>
      </div>
    </div>
    <div class="mobile-menu">
      <div class="logo-bar page-width">
        <div class="logo">
          <hpp-logo />
        </div>
        <div class="menu">
          <b-button v-b-toggle.sidebar-no-header class="side-bar-icon"
            ><img src="~/assets/icons/menuicon.svg" alt="Menu"
          /></b-button>

          <b-sidebar
            id="sidebar-no-header"
            aria-labelledby="sidebar-no-header-title"
            no-header
            shadow
          >
            <template #default="{ hide }">
              <div class="p-3">
                <a href="#!" class="cta-primary outlined small">Get a Quote</a>

                <nav class="mb-3">
                  <b-nav vertical>
                    <b-nav-item active @click="hide">Active</b-nav-item>
                    <b-nav-item href="#link-1" @click="hide">Link</b-nav-item>
                    <b-nav-item href="#link-2" @click="hide"
                      >Another Link</b-nav-item
                    >
                  </b-nav>
                </nav>
                <b-button variant="primary" block @click="hide"
                  >Close Sidebar</b-button
                >
              </div>
            </template>
          </b-sidebar>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import HppLogo from "../HppLogo.vue";
import Search from "./Search.vue";

export default {
  components: { Search, HppLogo },
  name: "HeaderMain",
  data: () => {
    return {
      drawer: null,
      items: [
        { title: "Home", icon: "mdi-view-dashboard" },
        { title: "About", icon: "mdi-forum" },
      ],
      serviceOpen: false,
      aboutOpen: false,
      insightOpen: false,
      solutionOpen: false,
      solutionOpenNew: false,
      industryOpen: false,
      industryOpennew: false,
      serviceOpenNew: false,
    };
  },
  methods: {
    openService() {
      (this.solutionOpen = false),
        (this.industryOpen = false),
        (this.industryOpennew = false),
        (this.serviceOpenNew = false),
        (this.serviceOpen = !this.serviceOpen);
    },
    openAbout() {
      this.solutionOpen = false;
      this.industryOpen = false;
      this.serviceOpen = false;
      this.serviceOpenNew = false;
      this.aboutOpen = !this.aboutOpen;
    },
    openInsight() {
      this.solutionOpen = false;
      this.industryOpen = false;
      this.serviceOpen = false;
      this.serviceOpenNew = false;
      this.aboutOpen = false;
      this.insightOpen = !this.insightOpen;
    },
    openServiceNew() {
      this.solutionOpen = false;
      this.industryOpen = false;
      this.serviceOpen = false;
      this.serviceOpenNew = !this.serviceOpenNew;
    },
    openIndustryOpen() {
      this.serviceOpen = false;
      this.solutionOpen = false;
      this.industryOpen = !this.industryOpen;
    },
    openIndustryOpenNew() {
      this.serviceOpen = false;
      this.solutionOpen = false;
      this.solutionOpenNew = false;
      this.industryOpennew = !this.industryOpennew;
    },
    openSolution() {
      this.serviceOpen = false;
      this.industryOpen = false;
      this.solutionOpen = !this.solutionOpen;
    },
    openSolutionNew() {
      this.serviceOpen = false;
      this.industryOpen = false;
      this.industryOpennew = false;
      this.solutionOpenNew = !this.solutionOpenNew;
    },
    checkDrawer() {
      if (this.drawer === false) {
        this.serviceOpen = false;
        this.solutionOpen = false;
        this.industryOpen = false;
        this.aboutOpen = false;
        this.insightOpen = false;
      }
    },
    closeMega() {
      return;
      if (
        this.serviceOpen == true ||
        this.solutionOpen == true ||
        this.aboutOpen == true ||
        this.industryOpen == true
      ) {
        this.serviceOpen = false;
        this.solutionOpen = false;
        this.industryOpen = false;
        this.aboutOpen = false;
      }
    },
  },
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

.mobile-menu {
  display: none;
}
.desktop-header {
  display: block;
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
.v-navigation-drawer {
  z-index: -1;
  width: 85vw !important;
}
.menu-container {
  padding: 20px;
  padding-top: 120px;
  .menu {
    list-style-type: none;
    .menu-item {
      font-size: 28px;
      margin-bottom: 15px;
      position: relative;
      a {
        color: black;
        display: block;
        cursor: pointer;
      }
      img {
        width: 12px;
        box-sizing: content-box;
        padding-left: 50px;
        cursor: pointer;
      }
    }
    .menu-item.sub-menu-item {
      display: flex;
      justify-content: space-between;
      a {
        flex: 1;
      }
    }
    .menu-item.sub-menu-item.services {
      display: flex;
      justify-content: space-between;
      a {
        flex: 0;
      }
      img {
        width: 12px;
      }
    }
  }
}

@media (max-width: 480px) {
  .desktop-header {
    display: none;
  }
  .mobile-menu {
    display: block;
    margin-bottom: 25px;

    .menu {
      .side-bar-icon {
        background: none;
        border: none;
      }

      a {
        width: 100%;
        text-align: center;
      }
    }
  }
}
</style>