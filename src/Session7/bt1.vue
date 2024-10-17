<template>
    <div>
        <h1>Childrent Company: {{ title }}</h1>
    </div>
</template>

<script setup lang="ts">
defineProps ({
    title: {
        type: String,
        default: "Rikkei Academy"
    }
})
</script>

<style scoped>

</style>