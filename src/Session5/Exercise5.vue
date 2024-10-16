<template>
    <div>
        <p>Các số chẵn trong mảng là: {{ filterNumber() }}</p>

    </div>
</template>

<script setup lang="ts">
let array = [1,2,3,4,5,6,7,8,9,10]

let filterNumber = () => {
    return array.filter(number => number % 2 === 0);
}
</script>

<style scoped>

</style>