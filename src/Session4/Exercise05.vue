<template>
    <div>
      <span>Cam: {{ product1.type }} - Số Lượng: {{ product1.quantity }}</span>
      <button @click="increaseQuantity(1)">Tăng số lượng</button>
      <br>
      <span>Táo: {{ product2.type }} - Số Lượng: {{ product2.quantity }}</span>
      <button @click="increaseQuantity(2)">Tăng số lượng</button>
      <br>
      <span>Nho: {{ product3.type }} - Số Lượng: {{ product3.quantity }}</span>
      <button @click="increaseQuantity(3)">Tăng số lượng</button>
      <br>
  
      <h1>Tổng số lượng sản phẩm: {{ totalQuantity }}</h1>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref, computed } from 'vue';
  
  let product1 = ref({
    type: "Cam",
    quantity: 4,
  });
  
  let product2 = ref({
    type: "Táo",
    quantity: 5,
  });
  
  let product3 = ref({
    type: "Nho",
    quantity: 3,
  });

  let increaseQuantity = (productType: number) => {
    if (productType === 1) {
      product1.value.quantity++;
    } else if (productType === 2) {
      product2.value.quantity++;
    } else if (productType === 3) {
      product3.value.quantity++;
    }
  };
  
  let totalQuantity = computed(() => {
    return product1.value.quantity + product2.value.quantity + product3.value.quantity;
  });
  </script>
  
  <style scoped>
  </style>
  