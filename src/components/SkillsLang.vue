<template>
  <section id="skills" class="skills-mf sect-pt4 route">
    <div class="container box-shadow-full" data-aos="fade-up">
      <div class="row">
        <div class="col-sm-12">
          <div class="title-box-2">
              <h5 class="title-left">
                Programming Skills
              </h5>
            </div>
        </div>
      </div>
      <div class="row row-skills">
        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/php.png" class="img-fluid img-skill" alt="PHP logo" title="PHP"/>
            </div>
          </div>
        </div>

        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/vuejs.png" class="img-fluid img-skill" alt="Vue.js logo" title="Vue.js"/>
            </div>
          </div>
        </div>

        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/laravel.png" class="img-fluid img-skill" alt="Laravel logo" title="Laravel"/>
            </div>
          </div>
        </div>

        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/html5.png" class="img-fluid img-skill" alt="HTML5 logo" title="HTML5"/>
            </div>
          </div>
        </div>

        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/css.png" class="img-fluid img-skill" alt="CSS logo" title="CSS"/>
            </div>
          </div>
        </div>

        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/javascript.png" class="img-fluid img-skill" alt="JavaScript logo" title="JavaScript"/>
            </div>
          </div>
        </div>

      </div>

      <div class="row row-skills mt-4">
        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/cplusplus.png" class="img-fluid img-skill" alt="PHP logo" title="PHP"/>
            </div>
          </div>
        </div>

        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/csharp.png" class="img-fluid img-skill" alt="Vue.js logo" title="Vue.js"/>
            </div>
          </div>
        </div>

        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/java.png" class="img-fluid img-skill" alt="Laravel logo" title="Laravel"/>
            </div>
          </div>
        </div>

        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/bootstrap.png" class="img-fluid img-skill" alt="HTML5 logo" title="HTML5"/>
            </div>
          </div>
        </div>

        <div class="col-md-2">
          <div class="work-img">
            <div class="row">
                <img src="../assets/mysql.png" class="img-fluid img-skill" alt="CSS logo" title="CSS"/>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.img-skill {
  width: 150px;
  transition: transform 500ms;
}

.img-skill:hover{
  transform: scale(1.1);
}

.row{
  justify-content: center !important;
}

.skills-mf .box-shadow-full {
  padding-top: 4rem;
  padding-bottom: 4rem;
}

.box-shadow-full {
  padding: 3rem 1.25rem;
  position: relative;
  background-color: #ffffff;
  margin-bottom: 3rem;
  z-index: 2;
  box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.06), 0 2px 5px 0 rgba(0, 0, 0, 0.2);
}

.title-box-2 {
  margin-bottom: 3rem;
}

.title-left {
  font-size: 2rem;
  position: relative;
}

.title-left:before {
  content: '';
  position: absolute;
  height: 3px;
  background-color: #0078ff;
  width: 100px;
  bottom: -12px;
}

</style>