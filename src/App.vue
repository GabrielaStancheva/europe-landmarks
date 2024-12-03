<template>
  <div id="app">
    <MainHeader />
    <LandmarkList :landmarks="landmarks" />
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import LandmarkList from './components/LandmarkList.vue';

export default {
  name: 'App',
  components: {
    MainHeader,  // Тук регистрираш MainHeader
    LandmarkList
  },
  data() {
    return {
      landmarks: [
        { name: "Eiffel Tower", country: "France", description: "Iconic Parisian landmark." },
        { name: "Colosseum", country: "Italy", description: "Ancient Roman amphitheater." },
        { name: "Big Ben", country: "United Kingdom", description: "Famous London clock tower." },
        { name: "Sagrada Familia", country: "Spain", description: "Gaudí’s masterpiece in Barcelona." }
      ]
    };
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 20px;
}
</style>
