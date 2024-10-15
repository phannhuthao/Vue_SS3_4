<template>
    <div>
        <input type="text" :disabled="isDisable">
    </div>
</template>

<script setup lang="ts">
let isDisable: boolean = true
</script>

<style scoped>

</style>