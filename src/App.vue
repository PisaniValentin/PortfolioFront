<script setup>
import { RouterLink, RouterView } from 'vue-router'
import InformationComponent from './components/InformationComponent.vue';
</script>

<template>
  <header class="row">
    <div class="col-6">
      <InformationComponent />
      <div class="wrapper">
        <nav>
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
        </nav>
      </div>
    </div>
    <div class="col-6 routerContainer">
      Descripcion
      <RouterView />
    </div>
  </header>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

header {
  line-height: 1.5;
  max-height: 100vh;
}

.routerContainer {
  background: white;
  height: 60vh;
  margin-top: 10vh;
  width: 60%;
}

</style>
