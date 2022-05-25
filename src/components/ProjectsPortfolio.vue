<template>
  <section id="work" class="portfolio-mf sect-pt4 route">
    <div class="container box-shadow-full" data-aos="fade-up">
      <div class="row">
        <div class="col-sm-12">
          <div class="title-box text-center">
            <h3 class="title-a">Portfolio</h3>
            <p class="subtitle-a">Some of my work done so far</p>
            <div class="line-mf"></div>
          </div>
        </div>
      </div>
      <div
        id="carouselProjects"
        class="carousel carousel-dark slide"
        data-bs-ride="carousel"
      >
        <div class="carousel-indicators">
          <button
            type="button"
            data-bs-target="#carouselProjects"
            data-bs-slide-to="0"
            class="active"
            aria-current="true"
            aria-label="Slide 1"
          ></button>
          <button
            type="button"
            data-bs-target="#carouselProjects"
            data-bs-slide-to="1"
            aria-label="Slide 2"
          ></button>
          <button
            type="button"
            data-bs-target="#carouselProjects"
            data-bs-slide-to="2"
            aria-label="Slide 3"
          ></button>
          <button
            type="button"
            data-bs-target="#carouselProjects"
            data-bs-slide-to="3"
            aria-label="Slide 4"
          ></button>
        </div>
        <div class="carousel-inner pb-5">
          <div class="carousel-item active" data-bs-interval="false">
            <div class="carousel-element-centered">
              <img
                src="../assets/logo.svg"
                class="d-block w-50 mb-svg"
                alt="Broggi Logo"
                title="Broggi"
              />
              <div class="carousel-caption d-none d-md-block">
                <h5>iBroggi</h5>
                <div class="d-flex justify-content-center">
                  <p class="mr-p">Link to this project's</p>
                  <a href="https://github.com/DevinSJ/project-broggi.git" target="_blank" title="Link to GitHub project" >GitHub</a>
                  <p class="ml-p">repository</p>
                </div>
              </div>
            </div>
          </div>
          <div class="carousel-item" data-bs-interval="500000">
            <div class="carousel-element-centered">
              <img
                src="../assets/cazaFrase2.png"
                class="d-block w-50 mb-png"
                alt="Caza Frase in-game"
                title="PacMan"
              />
              <div class="carousel-caption d-none d-md-block">
                <h5>CazaFrase</h5>
                <div class="d-flex justify-content-center">
                  <a
                    href="https://devinsj.github.io/CazaFrase/"
                    target="_blank"
                    title="Link to CazaFrase"
                    >Try it yourself!</a
                  >
                </div>
              </div>
            </div>
          </div>
          <div class="carousel-item" data-bs-interval="5000">
            <div class="carousel-element-centered">
              <img
                src="../assets/ecoarts.svg"
                class="d-block w-50 mb-svg"
                alt="EcoArts Logo"
                title="EcoArts"
              />
              <div class="carousel-caption d-none d-md-block">
                <h5>EcoArts</h5>
                <div class="d-flex justify-content-center">
                  <p class="mr-p">Link to this project's</p>
                  <a
                    href="https://github.com/x140l1n/ECOARTS-ANDROID.git"
                    target="_blank"
                    title="Link to GitHub project"
                    >GitHub</a
                  >
                  <p class="ml-p">repository</p>
                </div>
              </div>
            </div>
          </div>
          <div class="carousel-item" data-bs-interval="5000">
            <div class="carousel-element-centered">
              <img
                src="../assets/chrysallis.svg"
                class="d-block w-50 mb-svg"
                alt="Chrysallis Logo"
                title="Chrysallis"
              />
              <div class="carousel-caption d-none d-md-block">
                <h5>Chrysallis</h5>
                <div class="d-flex justify-content-center">
                  <p class="mr-p">Link to this project's</p>
                  <a
                    href="https://github.com/OriolMiralles/Projecte-Chrysallis.git"
                    target="_blank"
                    title="Link to GitHub project"
                    >GitHub</a
                  >
                  <p class="ml-p">repository</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <button
          class="carousel-control-prev"
          type="button"
          data-bs-target="#carouselProjects"
          data-bs-slide="prev"
        >
          <span class="carousel-control-prev-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button
          class="carousel-control-next"
          type="button"
          data-bs-target="#carouselProjects"
          data-bs-slide="next"
        >
          <span class="carousel-control-next-icon" aria-hidden="true"></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.box-shadow-full {
  padding: 3rem 1.25rem;
  position: relative;
  background-color: #ffffff;
  margin-bottom: 3rem;
  z-index: 2;
  box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.06), 0 2px 5px 0 rgba(0, 0, 0, 0.2);
}

.carousel-element-centered {
  display: flex;
  justify-content: center;
}

@media (min-width: 769px) {
  .mb-svg {
    margin-bottom: 150px;
  }
  .mb-png{
    margin-bottom: 170px;
  }
}

.mr-p {
  margin-right: 5px;
}

.ml-p {
  margin-left: 5px;
}

.title-a {
  text-decoration: none;
  font-size: 3rem;
  font-weight: bold;
  text-transform: uppercase;
}

.title-left {
  font-size: 2rem;
  position: relative;
}

.title-left:before {
  content: "";
  position: absolute;
  height: 3px;
  background-color: #0078ff;
  width: 100px;
  bottom: -12px;
}

.line-mf {
  width: 10%;
  height: 3px;
  background-color: #0078ff;
  margin: -10px auto 10px;
}

</style>