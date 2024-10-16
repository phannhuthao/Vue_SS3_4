<script setup lang="ts">
import { ref, computed, watch } from 'vue';
import Exercise1 from './Session5/Exercise1.vue';
import Exercise2 from './Session5/Exercise2.vue';
import Exercise3 from './Session5/Exercise3.vue';
import Exercise4 from './Session5/Exercise4.vue';
import Exercise5 from './Session5/Exercise5.vue';
import Exercise6 from './Session5/Exercise6.vue';
import Exercise7 from './Session5/Exercise7.vue';

// let isShow = ref(0);
// let userList = [
//   {
//     id:1,
//     userName:"admin",
//     password: "123",
//     gender: false
//   },

//   {
//     id: 2,
//     userName: "user",
//     password: "456",
//     gender: true
//   }
// ]
</script>


<template>

  <!-- <Exercise1/> -->
   <!-- <Exercise2/> -->
    <!-- <Exercise3/> -->
     <!-- <Exercise4/> -->
      <!-- <Exercise5/> -->
       <!-- <Exercise6/> -->
        <Exercise7/>

  <!-- <div v-if="isShow == 0">Xin chào</div>
  <div v-else-if="isShow == 1">Nhìn cc</div>
  <div v-else>Tạm biệt</div>
  <br>
  <button @click="() => {
    isShow = isShow == 0 ? 1 : 0;
  }" >Show</button>

  <button @click="() => {
    isShow = 2;
  }">Show Other</button>


  <div v-show="false">Nakano Nino</div> -->

  <!-- <table class="bang">
    <thead>
      <tr>
        <th>STT</th>
        <th>Name</th>
        <th>Password</th>
        <th>Gender</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(user, index) in userList" :key ="user.id">
        <th>{{ index + 1 }}</th>
        <th>{{ user.userName }}</th>
        <th>{{ user.password }}</th>
        <th>{{ user.gender  }}</th>
      </tr>
    </tbody>
  </table> -->
  
  </template>

<style scoped>
 /* table, th, td, tr {
    border: 1px solid black;
    border-collapse: collapse;
    text-align: center;
  } */

</style>
