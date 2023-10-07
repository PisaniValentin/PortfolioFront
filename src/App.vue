<script setup>
import InformationComponent from './components/InformationComponent.vue';
import ProjectSection from './components/ProjectsSection.vue';
import GithubComponent from './components/GithubComponent.vue';
import AboutMeComponent from './components/AboutMeComponent.vue';
</script>

<template>
  <main class="row">
    <div class="col-4 informationContainer">
      <InformationComponent />
      <GithubComponent />
      <!--
        <div class="wrapper">
          <nav>
            <RouterLink to="/">Home</RouterLink>
            <RouterLink to="/about">About</RouterLink>
          </nav>
        </div>
      -->
    </div>
    <div class="col-7">
      <div class="sectionContainer">
        <AboutMeComponent />
      </div>
      <div class="sectionContainer">
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
  line-height: 1.5;
  min-height: 100vh;
  background: #c9c5bd;
  padding-top: 20px;
}

.sectionContainer {
  display: flex;
  justify-content: start;
  flex-direction: column;
  border-top-right-radius: 15px;
  border-bottom-right-radius: 15px;
  margin-left: 40px;
  margin-bottom: 10px;
  padding: 15px;
  background: #181818;
}
</style>
