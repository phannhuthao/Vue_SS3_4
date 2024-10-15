<template>
    <div>
      <input type="text" v-model="inputValue" />
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref, watch } from 'vue';
  let inputValue = ref("");
  
  watch(inputValue, (newValue, oldValue) => {
    console.log(`Giá trị đã thay đổi từ "${oldValue}" thành "${newValue}"`);
  });
  </script>
  
  <style scoped>
  </style>
  