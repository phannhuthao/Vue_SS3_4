<template>
    <div>
      <input type="number" v-model.number="inputValue" />
      <button @click="addToCart">Add to cart</button>
  
      <p>Tổng số tiền trong giỏ hàng: {{ totalPrice }}</p>
      <p>Giá trị hiện tại từ input: {{ inputValue }}</p>
      <p>Giá trị bình phương của số hiện tại: {{ squaredValue }}</p>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref, computed, watch } from 'vue';
  
  let inputValue = ref(0);
  let totalCartPrice = ref(0);
  
  let squaredValue = computed(() => {
    return inputValue.value * inputValue.value;
  });
  
  watch(inputValue, (newValue) => {
    console.log(`Giá trị mới: ${newValue}`);
  });
  
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
  