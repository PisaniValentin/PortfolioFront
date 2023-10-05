<script setup>
import { RouterLink, RouterView } from 'vue-router'
import InformationComponent from './components/InformationComponent.vue';
</script>

<template>
  <header class="row">
    <div class="col-4 informationContainer">
      <InformationComponent />
      <div class="wrapper">
        <nav>
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
        </nav>
      </div>
    </div>
    <div class="col-8 routerContainer">
      <div class="">
        <RouterView />
      </div>
    </div>
  </header>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.informationContainer {
  padding: 15px;
  display: flex;
  justify-content: center;
}

.routerContainer>div {
  height: 100%;
  width: 100%;
  background: rgb(0, 0, 0);
  border-radius: 15px;
  border:2px solid rgb(255, 227, 69);
  padding: 20px;
}

header {
  line-height: 1.5;
  max-height: 100vh;
  background: rgb(0, 0, 0);
  background: linear-gradient(52deg, rgba(0, 0, 0, 1) 3%, rgba(30, 7, 57, 1) 27%, rgba(118, 0, 255, 1) 100%, rgba(49, 11, 94, 1) 100%);
}

.routerContainer {
  height: 70vh;
  border-radius: 10px;
  padding: 15px;

}
</style>
