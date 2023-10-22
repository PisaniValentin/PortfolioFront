<script setup>
import ProjectSection from './components/ProjectsSection.vue';
import AboutMeComponent from './components/AboutMeComponent.vue';
import SocialMediaComponent from './components/SocialMediaComponent.vue';
</script>


<template>
  <main class="container">
    <div class="aboutMeContainer">
      <AboutMeComponent />
    </div>
    <div class="projectContainer">
      <ProjectSection />
      <SocialMediaComponent />
    </div>
  </main>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


@media (max-width: 321px) {
  SocialMediaComponent {
    display: flex;
    visibility: none;
  }


}

main {
  min-height: 100vh;
  width: 100vw;
  background-image: linear-gradient(to bottom, #150a29, #19051d, #170213, #100008, #000000);
  padding: 30px;
}

.projectContainer {
  height: 100%;
}
</style>
