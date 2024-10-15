<template>
    <div>
      <a href="https://www.google.com" @click="checkUrl">Nhấp vào đi bạn</a>
    </div>
  </template>
  
  <script setup lang="ts">
  const checkUrl = (event: Event) => {
    const target = event.target as HTMLAnchorElement;
    const url = target.href;
  
    if (!url.startsWith("https://")) {
      event.preventDefault();
      alert("Đường dẫn không hợp lệ");
    }
  };
  </script>
  
  <style scoped>
  </style>
  