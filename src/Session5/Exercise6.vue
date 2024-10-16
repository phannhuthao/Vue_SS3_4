<template>
    <div>
        <p class="tittle">Danh sách các số đạt đủ điều kiện: {{ filterNumberNguyen() }}</p>
    </div>
</template>

<script setup lang="ts">
let array = [5, 12, 15, 22, 9, 18, 25, 30, 7, 33];

let filterNumberNguyen = () => {
    return array.filter(number => number % 2 === 0);
}
</script>

<style scoped>
.tittle {
    text-align: center;
    font-size: 20px;
}
</style>
