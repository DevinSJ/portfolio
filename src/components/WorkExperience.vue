<template>
  <section id="experience" class="about-mf sect-pt4 route">
      <div class="container">
        <div class="row">
          <div class="col-sm-12">
            <div class="box-shadow-full">
              <div class="title-box text-center">
                <h3 class="title-a">
                  Experience
                </h3>
                <p class="subtitle-a">
                  My laboral experience.
                </p>
                <div class="line-mf"></div>
              </div>
              <div class="row">
                <div class="col-lg-6">


                  <h3 class="resume-title">Education</h3>
                  <hr>
                  <div class="resume-item">
                    <h4>Certificate of Higher Education - DAW</h4>
                    <h5>2021 - 2022</h5>
                    <p><em>Centre d'Estudis Politècnics, Barcelona</em></p>
                    <p>On this extra course, I've accomplished both multiplatform and web development and so I obtained
                      a lot of knowledge about different web development languages such as HTML, CSS, Javascript and
                      also
                      PHP, Laravel and Vue.js.
                    </p>
                  </div>
                  <div class="resume-item">
                    <h4>Certificate of Higher Education - DAM</h4>
                    <h5>2019 - 2021</h5>
                    <p><em>Centre d'Estudis Politècnics, Barcelona</em></p>
                    <p>I've learned object-oriented programming, designing mobile applications and also desktop
                      applications. I also learned to design APIs and notions of the Web (HTML and CSS).</p>
                  </div>
                  <div class="resume-item">
                    <h4>General Certificate of Education</h4>
                    <h5>2015 - 2017</h5>
                    <p><em>INS Joan Coromines, Pineda de Mar, Barcelona</em></p>
                    <p>I did the subjects of "Batxillerat Tecnològic" and as optional subjects I decided to give a try
                      to physics,
                      computer science and technology.</p>
                  </div>
                </div>
                <div class="col-lg-6">
                  <h3 class="resume-title">Professional Experience</h3>
                  <hr>
                  <div class="resume-item">
                    <h4>Web development and maintenance</h4>
                    <h5>2021 - 2022</h5>
                    <p><em>Ormon Global</em></p>
                    <ul>
                      <li>I have been in this company working on the development and maintenance of their web. Worked
                        with
                        HTML, CSS, JavaScript as well as with PHP and Laravel.
                      </li>
                    </ul>
                  </div>
                  <div class="resume-item">
                    <h4>App Development for real clients</h4>
                    <h5>2021</h5>
                    <p><em>Centre d'Estudis Politècnics, Barcelona</em></p>
                    <ul>
                      <li>Developed a Desktop Application in C# to manage different types of events and users of
                        Chrysallis as well
                        as an Android Application in Java and XML for users and partners.</li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
     name: "WorkExperienceComponent"
};
</script>

<style scoped>
.box-shadow-full {
  padding: 3rem 1.25rem;
  position: relative;
  background-color: #fff;
  margin-bottom: 3rem;
  z-index: 2;
  box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.06), 0 2px 5px 0 rgba(0, 0, 0, 0.2);
}

.title-box {
  margin-bottom: 4rem;
}

.title-a {
  text-decoration: none;
  font-size: 3rem;
  font-weight: bold;
  text-transform: uppercase;
}

.subtitle-a {
  text-decoration: none;
  color: #4e4e4e;
}

.subtitle-a {
  text-decoration: none;
  color: #4e4e4e;
}

.line-mf {
  width: 40px;
  height: 5px;
  background-color: #0078ff;
  margin: 0 auto;
}

.resume-item {
  margin-bottom: 50px;
}

.resume .resume-item {
  padding: 0 0 20px 20px;
  margin-top: -2px;
  border-left: 2px solid #0563bb;
  position: relative;
  
}

.resume .resume-item h4 {
  line-height: 18px;
  font-size: 18px;
  font-weight: 600;
  text-transform: uppercase;
  font-family: "Poppins", sans-serif;
  color: #0563bb;
  margin-bottom: 10px;
}

.resume .resume-item h5 {
  font-size: 16px;
  background: #f7f8f9;
  padding: 5px 15px;
  display: inline-block;
  font-weight: 600;
  margin-bottom: 10px;
}

.resume .resume-item ul {
  padding-left: 20px;
}

.resume .resume-item ul li {
  padding-bottom: 10px;
}

.resume .resume-item:last-child {
  padding-bottom: 0;
}

.resume .resume-item::before {
  content: "";
  position: absolute;
  width: 16px;
  height: 16px;
  border-radius: 50px;
  left: -9px;
  top: 0;
  background: #fff;
  border: 2px solid #0078ff;
}

li{
  list-style-type: none;
}
</style>