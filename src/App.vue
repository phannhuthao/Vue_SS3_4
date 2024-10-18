<script setup lang="ts">
import { ref, watch } from 'vue';
import Exercise01 from './Session9/Exercise01.vue';
import Exercise02 from './Session9/Exercise02.vue';
import Exercise03 from './Session9/Exercise03.vue';
import Exercise04 from './Session9/Exercise04.vue';
import Exercise05 from './Session9/Exercise05.vue';
import Exercise06 from './Session9/Exercise06.vue';
import Exercise07 from './Session9/Exercise07.vue';

// let count = ref(0);
// let message = ref('gia tri message');

// watch(message, (newVal, olVal) => {
//   console.log("message change", newVal, olVal)
// })
</script>

<template>
<!-- <p>Count: {{ count }}</p>
<input type="text" :value="message" @change="(e) => {
  console.log('Giá trị:', e.target.value)
}"></input> -->

<!-- <form action="">
  <p>User Name:</p>
  <input type="text" placeholder="user name"></input>
  <br>

  <p>Password</p>
</form> -->
<Exercise07/>

</template>




<style scoped>

</style>
