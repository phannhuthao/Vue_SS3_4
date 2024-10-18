<template>
    <div>
      <p>Sở thích: [ {{ favorite.join(', ') }} ]</p>
      <br>
      <input type="checkbox" v-model="favorite" value="Bóng đá" /> Bóng đá
      <br>
      <input type="checkbox" v-model="favorite" value="Bóng rổ" /> Bóng rổ
      <br>
      <input type="checkbox" v-model="favorite" value="Bóng bầu dục" /> Bóng bầu dục
      <br>
      <input type="checkbox" v-model="favorite" value="Bóng chày" /> Bóng chày
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  
  let favorite = ref<Array<string>>([]);
  </script>
  
  <style scoped>
  </style>
  