<script setup>
import InformationComponent from './components/InformationComponent.vue';
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
  width: 100%;
  line-height: 1.5;
  min-height: 100%;
  background: #c9c5bd;
  padding: 20px;
}

.projectContainer {
  display: flex;
  justify-content: start;
  flex-direction: column;
  margin-bottom: 10px;
}

.aboutMeContainer{
  display: flex;
  justify-content: start;
  flex-direction: column;
  margin-bottom: 10px;
  padding-right: 30px;
}
</style>
