<script setup>
import ProjectSection from './components/ProjectsSection.vue';
import GithubComponent from './components/GithubComponent.vue';
import AboutMeComponent from './components/AboutMeComponent.vue';
</script>

<template>
  <main class="row">
    <div class="col-4 informationContainer">
      <div class="aboutMeContainer">
        <AboutMeComponent />
        <GithubComponent />
      </div>
    </div>
    <div class="col-8">
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

.informationContainer {
  display: flex;
  flex-direction: column;
  justify-content: start;
}

main {
  width: 100vw;
  min-height: 100vh;
  line-height: 1.5;
  background: #c9c5bd;
  padding: 20px;
}

.projectContainer {
  height: 100%;
}

.aboutMeContainer{
  height: 100%;
  display: flex;
  flex-direction: column;
  padding-right: 30px;
}
</style>
