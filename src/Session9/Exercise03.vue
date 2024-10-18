<template>
    <div>
        <p>Ngày sinh: {{ date }}</p>
        <input type="date" v-model="date" ></input>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

let date = ref('');

</script>

<style scoped>

</style>