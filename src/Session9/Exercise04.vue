<template>
    <div>
        <p>Tiến độ hoàn thành: {{ range }} %</p>
        <input type="range" v-model="range" ></input>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

let range = ref('');

</script>

<style scoped>

</style>