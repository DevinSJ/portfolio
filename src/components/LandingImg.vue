<template>
  <div id="landing" class="hero route bg-image">
    <div class="overlay-itro"></div>
    <div class="hero-content display-table">
      <div class="table-cell">
        <div class="container">
          <h1 class="hero-title mb-4">
            Hey! I'm <span class="text-remarked">Devin</span> Schlippe
          </h1>
        </div>
        <div class="div-typed">
          <vue-typed-js
            :strings="['Full Stack Developer']"
            :loop="true"
            :typeSpeed="100"
            :backSpeed="100"
            :autoInsertCss="true"
          >
            <h1 class="typing"></h1>
          </vue-typed-js>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Vue from "vue";
import VueTypedJs from "vue-typed-js";

Vue.use(VueTypedJs);

export default {
  name: "LandingImgComponent",
};
</script>

<style scoped>
.hero {
  height: 100vh;
  position: relative;
  color: #ffffff;
}

.bg-image {
  background-image: url(../assets/fondo.png);
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
  background-position: center center;
}

.hero .hero-content {
  text-align: center;
  position: absolute;
}

.hero .overlay-itro {
  background-color: rgba(0, 0, 0, 0.6);
  position: absolute;
  top: 0;
  left: 0px;
  padding: 0;
  height: 100%;
  width: 100%;
  opacity: 0.9;
}

.hero .hero-title {
  color: #ffffff;
  font-weight: 600;
  font-size: 3rem;
}

@media (min-width: 768px) {
  .hero .hero-title {
    font-size: 4.5rem;
  }
}

.hero .hero-subtitle {
  font-size: 1.5rem;
  font-weight: 600;
}

@media (min-width: 768px) {
  .hero .hero-subtitle {
    font-size: 2.5rem;
  }
}

.hero .text-slider-items {
  display: none;
}

.hero-single {
  height: 350px;
}

.hero-single .hero-content {
  margin-top: 30px;
}

.hero-single .hero-title {
  text-transform: uppercase;
  font-size: 3rem;
}

@media (min-width: 768px) {
  .hero-single .hero-title {
    font-size: 3.5rem;
  }
}

.hero-single .breadcrumb {
  background-color: ransparent;
  color: #0078ff;
}

.hero-single .breadcrumb .breadcrumb-item:before {
  color: #ffffff;
}

.hero-single .breadcrumb .breadcrumb-item.active {
  color: #ffffff;
}

.hero-single .breadcrumb a {
  color: #ffffff;
}

.hero .overlay-itro {
  background-color: rgba(0, 0, 0, 0.6);
  position: absolute;
  top: 0;
  left: 0px;
  padding: 0;
  height: 100%;
  width: 100%;
  opacity: 0.9;
}

.display-table {
  width: 100%;
  height: 100%;
  display: table;
}

.table-cell {
  display: table-cell;
  vertical-align: middle;
}

.text-remarked {
  position: relative;
}

.text-remarked::before {
  content: "";
  position: absolute;
  height: 5px;
  background-color: #0078ff;
  width: 100%;
  bottom: -5px;
  animation: spanding 5s infinite;
  transform-origin: 0% 100%;
}

@keyframes spanding {
  0% {
    transform: scaleX(0);
  }
  50% {
    transform: scaleX(1);
  }
  100% {
    transform: scaleX(0);
  }
}

::v-deep .typed-cursor {
  font-size: 50px;
}

.div-typed {
  display: flex;
  justify-content: center;
}
</style>