<template>
    <div>
      <span>Chiều dài: {{ width }}</span>
      <br>
      <span>Chiều rộng: {{ height }}</span>
      <br>
      <span>Diện tích: {{ dienTich }}</span>
      <br>
      <button @click="increaseWidth">Increase width</button>
    </div>
  </template>
  
  <script setup lang="ts">
  import { computed, ref } from 'vue';
  let width = ref(10);
  let height = ref(20);
  
  let dienTich = computed(() => {
    return width.value * height.value;
  });
  
  let increaseWidth = () => {
    width.value += 10;
  };
  </script>
  
  <style scoped>
  </style>
  