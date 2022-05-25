<template>
  <div class="home">
    <NavBar />
    <LandingImgComponent />
    <AboutMe />
    <SkillLang />
    <ProjectsPortfolio />
    <WorkExperience />
    <ContactMe />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue'
import LandingImgComponent from '@/components/LandingImg.vue'
import AboutMe from '@/components/AboutMe.vue'
import SkillLang from '@/components/SkillsLang.vue'
import ProjectsPortfolio from '@/components/ProjectsPortfolio.vue'
import WorkExperience from '@/components/WorkExperience.vue'
import ContactMe from '@/components/ContactMe.vue'

export default {
  name: 'HomeView',
  components: {
    NavBar,
    LandingImgComponent,
    AboutMe,
    SkillLang,
    ProjectsPortfolio,
    WorkExperience,
    ContactMe,
  }
}


</script>
