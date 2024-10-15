<template>
    <div>
        <span>Giá trị khởi tạo là: {{ soTinhTong }}</span>
        <br>
        <button @click="() => {
            number = number + 1
        }" >Click</button>
    </div> 
</template>

<script setup lang="ts">
import { computed, ref } from 'vue';
let number = ref(1);

let soTinhTong = computed(() => {
    return number.value + 1
})
</script>

<style scoped>

</style>