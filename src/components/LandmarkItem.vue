<template>
    <div class="landmark-item">
      <h3>{{ landmark.name }}</h3>
      <p><strong>Country:</strong> {{ landmark.country }}</p>
      <p>{{ landmark.description }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'LandmarkItem',
    props: {
      landmark: Object
    }
  };
  </script>
  
  <style scoped>
  .landmark-item {
    border: 1px solid #ddd;
    padding: 10px;
    margin: 10px 0;
    border-radius: 5px;
    background-color: #f9f9f9;
  }
  h3 {
    margin: 0;
  }
  </style>
  