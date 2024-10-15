<template>
    <div>
      <input type="number" v-model.number="inputValue" />
      <button @click="addToCart">Add to cart</button>
  
      <p>Tổng số tiền trong giỏ hàng: {{ totalPrice }}</p>
      <p>Giá trị hiện tại từ input: {{ inputValue }}</p>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref, computed } from 'vue';
  
  let inputValue = ref(0);
  let totalCartPrice = ref(0);
  

  let addToCart = () => {
    totalCartPrice.value += inputValue.value;
    inputValue.value = 0; 
  };
  
  let totalPrice = computed(() => {
    return totalCartPrice.value;
  });
  </script>
  
  <style scoped>
  </style>
  