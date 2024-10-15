<template>
    <div>
      <span>{{ user.company }}</span><br>
      <span>{{ user.age }}</span><br>
  
      <button @click="handleChange">Change data</button>
    </div>
  </template>
  
  <script setup lang="ts">
  import { reactive } from 'vue';

  let user = reactive({
    company: "Rikkei Academy",
    age: 1
  });
  
  let handleChange = () => {
    user.company = "Rikkei Education";
    user.age = 2;
  };
  </script>
  
  <style scoped>
  </style>
  