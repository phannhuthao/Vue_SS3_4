<template>
    <div>    
        <button @click="handleClick">Get param</button>
    </div>
</template>

<script setup lang="ts">
let string = "Rikkei Academy"
let handleClick = () => {
    console.log(string);
}
</script>

<style scoped>

</style>