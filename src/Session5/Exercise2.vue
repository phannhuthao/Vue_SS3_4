<template>
    <div>
        <button class="button" @click="showHide">{{ isShow ? 'Ẩn' : 'Hiện' }}</button>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

let isShow = ref(true);

let showHide = () => {
    isShow.value = !isShow.value;
}
</script>

<style scoped>
.button {
    text-align: center;
    width: 50px;
    height: 50px;
}
</style>