<template>
    <div class="landmark-list">
      <h2>Landmarks</h2>
      <div v-for="landmark in landmarks" :key="landmark.name">
        <LandmarkItem :landmark="landmark" />
      </div>
    </div>
  </template>
  
  <script>
  import LandmarkItem from './LandmarkItem.vue';
  
  export default {
    name: 'LandmarkList',
    components: {
      LandmarkItem
    },
    props: {
      landmarks: Array
    }
  };
  </script>
  
  <style scoped>
  .landmark-list {
    margin-top: 20px;
  }
  </style>
  