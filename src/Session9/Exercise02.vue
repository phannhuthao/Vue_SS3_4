<template>
    <div>
        <input type="color" v-model="color" ></input>
        <p>Mã màu: {{ color }}</p>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

let color = ref('')
</script>

<style scoped>

</style>