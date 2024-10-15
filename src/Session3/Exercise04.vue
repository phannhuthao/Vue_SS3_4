<template>
    <div :class="{ active: isActive }" :style="{ backgroundColor: backgroundColor }">
      <h1>Block</h1>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  
  let isActive = ref(true); 
  let backgroundColor = ref('blue'); 
  </script>
  
  <style scoped>
  .active {
    color: #fff; 
  }
  
  div {
    color: black; 
    padding: 20px;
    border: 1px solid #000;
  }
  </style>
  