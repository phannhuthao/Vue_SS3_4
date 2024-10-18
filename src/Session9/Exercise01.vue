<template>
    <div>
      <p>Email: </p>
      <br>
      <input type="text" v-model="email" />
      <br>
      <p>Giá trị: {{ email }}</p>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  
  let email = ref('');
  </script>
  
  <style scoped>
  </style>
  