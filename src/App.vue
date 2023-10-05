<script setup>
import { RouterLink, RouterView } from 'vue-router'
import InformationComponent from './components/InformationComponent.vue';
import ProjectSection from './components/ProjectsSection.vue'
</script>

<template>
  <main class="row">
    <div class="col-4 informationContainer">
      <InformationComponent/>
      <!--
        <div class="wrapper">
          <nav>
            <RouterLink to="/">Home</RouterLink>
            <RouterLink to="/about">About</RouterLink>
          </nav>
        </div>
      -->
    </div>
    <div class="col-7 routerContainer">
      <RouterView />
    </div>
    <div>
      <ProjectSection/>
    </div>
    <div>
      TITLES SECTION
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
  justify-content: end;
}


main {
  width: 100vw;
  line-height: 1.5;
  min-height: 100vh;
  background: #c9c5bd;
  padding-top: 20px;
}

.routerContainer {
  display: flex;
  justify-content: start;
  height: 250px;
  border-top-right-radius: 15px;
  border-bottom-right-radius: 15px;
  margin-left: 40px;
  padding: 15px;
  background: #181818;
}
</style>
