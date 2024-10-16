<template>
    <h1 v-show="isVisible">Thông báo: Welcome to Rikkei Education</h1>
    <br>
    <button @click="showTitle">Hiển thị</button>
    <button @click="hideTitle">Ẩn</button>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';

  let isVisible = ref(false);
  
  let showTitle = () => {
    isVisible.value = true;
  };
  
  let hideTitle = () => {
    isVisible.value = false;
  };
  </script>
  
  <style scoped>
  button {
    margin-right: 10px;
  }
  </style>
  