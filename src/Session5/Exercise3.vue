<template>
    <div>
      <h1>Quyền hạn của bạn là: {{ getRoleName }}</h1>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref, computed } from 'vue';
  
  let role = ref('admin'); 
  
  let userRoles = [
    {
      role: 'user',
      name: 'Người dùng'
    },
    {
      role: 'admin',
      name: 'Quản trị viên'
    },
    {
      role: 'guest',
      name: 'Khách'
    }
  ];
  
  const getRoleName = computed(() => {
    const currentRole = userRoles.find(r => r.role === role.value);
    return currentRole ? currentRole.name : 'Không xác định';
  });
  </script>
  
  <style scoped>
  </style>
  