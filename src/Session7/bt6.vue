<!-- Card.vue -->
<template>
    <div class="card">
      <div class="card-header">
        <slot name="header"></slot>
      </div>
      <div class="card-body">
        <slot name="body"></slot>
      </div>
      <div class="card-footer">
        <slot name="footer"></slot>
      </div>
    </div>
  </template>
  
  <script setup lang="ts">
  
  </script>
  
  <style scoped>
  .card {
    border: 1px solid #ccc;
    border-radius: 8px;
    overflow: hidden;
    width: 300px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  .card-header,
  .card-footer {
    padding: 16px;
    border-bottom: 1px solid #ddd;
  }
  
  .card-body {
    padding: 16px;
  }
  
  .card-footer {
    border-top: 1px solid #ddd;
    text-align: right;
  }
  </style>
  