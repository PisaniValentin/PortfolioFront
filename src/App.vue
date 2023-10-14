<script setup>
import ProjectSection from './components/ProjectsSection.vue';
import GithubComponent from './components/GithubComponent.vue';
import AboutMeComponent from './components/AboutMeComponent.vue';
</script>

<template>
  <main class="row">
    <div class="col-sm-12 col-md-4 ">
      <div class="aboutMeContainer">
        <AboutMeComponent />
      </div>
    </div>
    <div class="col-sm-12 col-md-8">
      <div class="projectContainer">
        <ProjectSection />
      </div>
    </div>
  </main>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

@media (min-width: 320px){


}

.projectContainer {
  height: 100%;
}

main {
  width: 100vw;
  min-height: 100vh;
  line-height: 1.5;
  background-image: linear-gradient(to bottom, #150a29, #19051d, #170213, #100008, #000000);
  padding: 30px;
}
/**
 .aboutMeContainer {
    display: flex;
    flex-direction: column;
    height: 92%;
  }
*/
 
</style>
