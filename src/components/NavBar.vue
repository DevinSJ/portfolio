<template>
  <div>
    <nav id="navbar" class="navbar fixed-top navbar-expand-lg navbar-light">
      <div class="container-fluid">
        <a href="" title="Logo image" class="logoNavA"
          ><img
            src="../assets/logo.png"
            alt="Devin Schlippe Logo"
            title="Logo image"
            class="logoNav"
        /></a>
        <button
          id="btnShowMenu"
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
          @click="handleScreenWidthOnLoad"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a
                id="homeSection"
                class="nav-link text-white active"
                aria-current="page"
                href="#"
                title="home section"
                @click="changeActiveNav"
                >Home</a
              >
            </li>

            <li class="nav-item">
              <a
                id="aboutMeSection"
                class="nav-link text-white"
                href="#aboutme"
                title="about me section"
                @click="changeActiveNav"
                >About Me</a
              >
            </li>

            <li class="nav-item">
              <a
                id="skillsSection"
                class="nav-link text-white"
                href="#skills"
                title="about me section"
                @click="changeActiveNav"
                >Skills</a
              >
            </li>

            <li class="nav-item">
              <a
                id="workSection"
                class="nav-link text-white"
                href="#work"
                title="work section"
                @click="changeActiveNav"
                >Work</a
              >
            </li>

            <li class="nav-item">
              <a
                id="experienceSection"
                class="nav-link text-white"
                href="#experience"
                title="experience section"
                @click="changeActiveNav"
                >Experience</a
              >
            </li>

            <li class="nav-item">
              <a
                id="contactSection"
                class="nav-link text-white"
                href="#contact"
                title="contact section"
                @click="changeActiveNav"
                >Contact</a
              >
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <div class="button-div">
      <button @click="backToTop" class="button-top">
        <i class="fa-solid fa-arrow-up"></i>
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showMenu: false,
    };
  },
  name: "NavBarComponent",
  mounted() {
    this.handleScrollPosition();
    this.handleScreenWidthOnScroll();
  },
  methods: {
    handleScrollPosition() {
      window.onscroll = function () {
        let currentScroll = window.scrollY;
        let navbar = document.querySelector("#navbar");
        let buttonBackToTop = document.querySelector(".button-top");

        console.log(currentScroll);
        if (currentScroll > 200) {
          navbar.classList.add("nav-scrolled");
          buttonBackToTop.classList.add("show-button");
        } else {
          navbar.classList.remove("nav-scrolled");
          buttonBackToTop.classList.remove("show-button");
        }

        let navbarElements = document.querySelector(".navbar-nav").childNodes;

        if (currentScroll < 600) {
          navbarElements.forEach((element) => {
            if (element.childNodes[0].id == "homeSection") {
              element.childNodes[0].classList.add("active");
            } else {
              element.childNodes[0].classList.remove("active");
            }
          });
        } else if (currentScroll > 599 && currentScroll < 1399) {
          navbarElements.forEach((element) => {
            if (element.childNodes[0].id == "aboutMeSection") {
              element.childNodes[0].classList.add("active");
            } else {
              element.childNodes[0].classList.remove("active");
            }
          });
        } else if (currentScroll > 1399 && currentScroll < 1999) {
          navbarElements.forEach((element) => {
            if (element.childNodes[0].id == "skillsSection") {
              element.childNodes[0].classList.add("active");
            } else {
              element.childNodes[0].classList.remove("active");
            }
          });
        } else if (currentScroll > 1999 && currentScroll < 2699) {
          navbarElements.forEach((element) => {
            if (element.childNodes[0].id == "workSection") {
              element.childNodes[0].classList.add("active");
            } else {
              element.childNodes[0].classList.remove("active");
            }
          });
        } else if (currentScroll > 2699 && currentScroll < 3699) {
          navbarElements.forEach((element) => {
            if (element.childNodes[0].id == "experienceSection") {
              element.childNodes[0].classList.add("active");
            } else {
              element.childNodes[0].classList.remove("active");
            }
          });
        } else {
          navbarElements.forEach((element) => {
            if (element.childNodes[0].id == "contactSection") {
              element.childNodes[0].classList.add("active");
            } else {
              element.childNodes[0].classList.remove("active");
            }
          });
        }
      };
    },
    handleScreenWidthOnScroll() {
      window.onresize = function () {
        if (window.innerWidth < 992) {
          let navbarElement = document.querySelector("#navbarNav");
          let navBar = document.querySelector("#navbar");
          if (navbarElement.classList.contains("show")) {
            navBar.classList.add("navbar-bg");
          } else {
            navBar.classList.remove("navbar-bg");
          }
        }
      };
    },
    handleScreenWidthOnLoad() {
      this.showMenu = !this.showMenu;
      let navBar = document.querySelector("#navbar");
      if (this.showMenu) {
        navBar.classList.add("navbar-bg");
      } else {
        navBar.classList.remove("navbar-bg");
      }
    },
    changeActiveNav(event) {
      let navBarElements =
        event.currentTarget.parentElement.parentElement.childNodes;
      let currentNavItem = event.currentTarget;
      navBarElements.forEach((element) => {
        if (element.children[0].classList.contains("active")) {
          element.children[0].classList.remove("active");
        }
      });
      currentNavItem.classList.add("active");
    },
    backToTop() {
      window.scrollTo(0, 0);
    },
  },
};
</script>

<style scoped>
.logoNav {
  width: 50px;
}

@media (max-width: 991px) {
  .logoNavA {
    margin-left: 5%;
    padding-bottom: 5px;
  }
}

@media (min-width: 992px) {
  .nav-scrolled {
    background-color: #1e1e1e;
    opacity: 0.99;
    transition: 500ms;
  }

  .logoNavA {
    margin-left: 10%;
    padding-bottom: 5px;
  }
}

.nav-link:before {
  content: "";
  position: absolute;
  width: 100%;
  height: 2px;
  bottom: 0px;
  left: 0;
  width: 0;
  background-color: #ffffff;
  visibility: hidden !important;
  transition: all 0.3s ease-in-out 0s;
}

.nav-link {
  position: relative;
}

.nav-link:hover::before,
.nav-item .active:before {
  visibility: visible !important;
  width: 80%;
}

@media (max-width: 991px) {
  .navbar-toggler[aria-expanded="true"] .navbar {
    background-color: #1e1e1e;
    transition: 500ms;
  }

  .navbar-toggler[aria-expanded="false"] .navbar {
    background-color: #1e1e1e;
    transition: 500ms;
  }

  .navbar-bg {
    background-color: #1e1e1e;
    transition: 500ms;
  }

  .nav-link:before {
    content: "";
    position: absolute;
    width: 10% !important;
    height: 2px;
    bottom: 0px;
    left: 10;
    width: 0;
    background-color: #ffffff;
    visibility: hidden !important;
    transition: all 0.3s ease-in-out 0s;
  }
}

.navbar-collapse {
  text-transform: uppercase;
}

@media (min-width: 992px) {
  .navbar-collapse {
    justify-content: flex-end;
    padding-right: 15%;
  }
  nav a {
    margin-right: 20px;
    margin-top: 10px;
  }
}

.button-div {
  position: fixed;
  right: 20px;
  bottom: 20px;
  width: 40px;
  height: 40px;
  z-index: 996;
}

.button-top {
  background-color: #0078ff;
  border: 0;
  color: #ffffff;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  transition: 1s;
  display: none;
}

.show-button {
  display: block;
  pointer-events: auto;
}
</style>