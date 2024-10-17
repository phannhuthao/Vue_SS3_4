<template>
    <div>
        <li v-for="user in userList" :key="user.id">ID: {{ user.id }}</li>
        <li v-for="user in userList" :key="user.name">Name Product: {{ user.name }}</li>
        <li v-for="user in userList" :key="user.price">Price: {{ user.price }}</li>
        <li v-for="user in userList" :key="user.quantity">Quantity: {{ user.quantity }}</li>
        
    </div>
</template>

<script setup lang="ts">
import { defineProps, PropType } from 'vue';

interface User {
    id: number,
    name: string,
    price: number,
    quantity: number
}


defineProps ({
    userList: {
        type: Array as PropType<User[]>,
        required: true
    }
})
</script>

<style scoped>

</style>