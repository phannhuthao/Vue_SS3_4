<template>
    <div>
      <h1>Form</h1>
      <form @submit.prevent="handleSubmit">
        <input type="text" />
        <button type="submit">Submit</button>
      </form>
    </div>
  </template>
  
  <script setup lang="ts">
  const handleSubmit = () => {
    console.log("Form submission prevented!");
  };
  </script>
  
  <style scoped>
  </style>
  