<template>
    <div>
      <form class="form" @submit.prevent="addProduct">
        <h1>Thêm mới sản phẩm</h1>
        
        <div>
          <p>Mã sản phẩm</p>
          <input type="text" v-model="product.code" />
        </div>
  
        <div>
          <p>Tên sản phẩm</p>
          <input type="text" v-model="product.name" />
        </div>
  
        <div>
          <p>Giá</p>
          <input type="number" v-model="product.price" />
        </div>
  
        <div>
          <p>Số lượng</p>
          <input type="number" v-model="product.quantity" />
        </div>
  
        <br>
        <button class="button" type="submit">Thêm mới</button>
      </form>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  
  // Khởi tạo biến product chứa thông tin sản phẩm
  let product = ref({
    code: '',
    name: '',
    price: 0,
    quantity: 0,
  });
  
  // Hàm xử lý khi nhấn nút "Thêm mới"
  const addProduct = () => {
    console.log("Sản phẩm mới được thêm vào:", product.value);
    // Reset lại form sau khi thêm sản phẩm nếu cần
    product.value = {
      code: '',
      name: '',
      price: 0,
      quantity: 0,
    };
  };
  </script>
  
  <style scoped>
  .button {
    width: 150px;
    height: 30px;
    background-color: blue;
    color: white;
    border-radius: 4px;
    cursor: pointer;
  }
  
  .form {
    text-align: center;
  }
  </style>
  