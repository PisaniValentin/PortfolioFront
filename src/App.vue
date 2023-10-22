<script setup>
import ProjectSection from './components/ProjectsSection.vue';
import AboutMeComponent from './components/AboutMeComponent.vue';

</script>


<template>
  <main>
    <div class="AboutMeContainer">
      <AboutMeComponent />
    </div>
    <div class="projectContainer">
      <ProjectSection />
    </div>
  </main>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


@media (min-width: 320px) {}

@media (min-width: 768px) {
  .projectContainer {
    height: 100%;
    width: 65vw;
    margin-left: 30vw;
  }
}

main {
  min-height: 100vh;
  width: 100vw;
  background-image: linear-gradient(to bottom, #150a29, #19051d, #170213, #100008, #000000);
  padding: 30px;
}
</style>
