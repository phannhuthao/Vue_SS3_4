<template>
    <div>
        <button @click="tittle" >Click Me</button>

    </div>
</template>

<script setup lang="ts">
let tittle = () => {
    console.log("Hello");
}
</script>

<style scoped>

</style>