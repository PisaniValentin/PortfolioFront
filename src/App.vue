<script setup>
import ProjectSection from './components/ProjectsSection.vue';
import AboutMeComponent from './components/AboutMeComponent.vue';
import TableButtons from './components/TableButtons.vue';
</script>


<template>
  <div class="general">
    <div class="mainContainer">
      <img src="./assets/mindhubRender4.png" class="background" alt="">
      <TableButtons />
    </div>
    <div class="monitor1">
      <h2>My projects</h2>
      <div class="projectContainer">
        <a href="">MINDHUB</a>
      </div>
      <div class="projectContainer">
        <a href="">MDHL Hockey League</a>
      </div>
      <div class="projectContainer">
        <a href="">Amazing Events</a>
      </div>
    </div>
  </div>
  <!--
  <main>
    <div class="AboutMeContainer">
      <AboutMeComponent />
    </div>
    <div class="projectContainer">
      <ProjectSection />
    </div>
  </main>
  -->
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.general {
  position: relative;
  display: flex;
  align-items: center;
  background: black;
  height: 100vh;
  width: 100vw;
}

@media (min-width: 320px) {}

@media (min-width: 768px) {
  .projectContainer {
    display: flex;
    justify-content: start;
    border: 1px solid black;
  }

  .projectContainer a {
    color: black;
    text-decoration: none;
  }

}

.mainContainer {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  color: black;
  background: black;
  height: 50vw;
  width: 100vw;
}

.background {
  width: 100%;
  height: 100%;
}

main {
  min-height: 100vh;
  width: 100vw;
  background-image: linear-gradient(to bottom, #150a29, #19051d, #170213, #100008, #000000);
  padding: 30px;
}

.monitor1 {
  position: absolute;
  z-index: 3;
  width: 304px;
  top: 89px;
  left: 285px;
  background: rgb(103, 159, 243);
  /* height: 303px; */
  color: black;
  perspective: 30px;
  transform: rotateY(360deg) rotateZ(342deg) rotateX(1deg);
}

.monitor2 img {
  width: 100%;
  height: 100%;
  right: 10px;
  top: 0px;
  width: 411px;
  height: 254px;
  transform: perspective(80px) rotateX(-1deg) rotateY(0deg) rotateZ(6deg);
}
</style>
