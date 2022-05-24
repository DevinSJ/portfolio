<template>
  <section id="aboutme" class="about-mf sect-pt4">
      <div class="container">
        <div class="row">
          <div class="col-sm-12">
            <div class="box-shadow-full">
              <div class="row">
                <div class="col-md-5">
                  <div class="row">
                    <div class="col-sm-6 col-md-8">
                      <div class="about-img">
                        <img src="../assets/mifoto.jpg" class="img-fluid rounded b-shadow-a" alt="Personal image">
                      </div>
                    </div>
                    <div class="col-sm-6 col-md-7 personal-data">
                        <p><span class="title-s">Name: </span> <span>Devin Schlippe</span></p>
                        <p><span class="title-s">Profile: </span> <span>Software Developer</span></p>
                        <p><span class="title-s">Email: </span> <span>devinschlippe@gmail.com</span></p>
                    </div>
                  </div>
                  
                </div>
                <div class="col-md-7">
                  <div class="about-me pt-4 pt-md-0">
                    <div class="title-box-2">
                      <h5 class="title-left">
                        About me
                      </h5>
                    </div>
                    <p class="lead">
                      Ever since I was a little kid, the informatic world has been my passion. I still remember that
                      christmas when I first got a computer and started
                      playing videogames like crazy, that was the moment I fell in love with Software.
                    </p>
                    <p class="lead">
                      Many years later I discovered something amazing, something that would mark my life and set a
                      trajectory in my actions and lifestyle. The first time
                      I programmed a "Hello World" in C++ made me go crazy. How was it possible that just by writting
                      few code lines I could get the computer to do
                      whatever I wanted.
                    </p>
                    <p class="lead">
                      This passion carried me through my education in Centre d'Estudis Politècnics, where I found more
                      resources available to me than I could
                      have ever imagined as a kid. I studied PHP, Html, C#, JavaScript among many other things but this
                      was the moment I realized how much there was yet to learn.
                    </p>
                    <p class="lead">
                      So, now that I am able to start my career in this world, this passion remains with me. I know
                      there are a lot of new things I still don't know about
                      their existence. But especially for this reason I am grateful and excited!
                    </p>
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

}
</script>

<style scoped>
.about-mf .box-shadow-full {
  padding-top: 4rem;
  padding-bottom: 4rem;
}

.about-mf .about-img {
  margin-bottom: 2rem;
}

.about-mf .about-img img {
  margin-left: 10px;
}

@media (min-width: 767px) {
  .about-mf .box-pl2 {
    margin-top: 3rem;
    padding-left: 0rem;
  }
}

.sect-pt4 {
  padding-top: 4rem;
}

.box-shadow-full {
  padding: 3rem 1.25rem;
  position: relative;
  background-color: #fff;
  margin-bottom: 3rem;
  z-index: 2;
  box-shadow: 0 1px 1px 0 rgba(0, 0, 0, 0.06), 0 2px 5px 0 rgba(0, 0, 0, 0.2);
}

.title-s {
  font-weight: 600;
  color: #1e1e1e;
  font-size: 1.1rem;
}

.personal-data{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding-left: 25px;
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

.lead{
    font-size: 1.25rem;
    font-weight: 300;
    text-align: justify;
    padding-right: 40px;
}
</style>