<template>
    <div>
        <!-- <h1>Đây là compent B</h1>
        <h3>Đây là count: {{ count }}</h3>
        <h3>Giá trị của test: {{ test }}</h3>
        <h3>Nội dung: {{ stringTittle }}</h3>

        <li v-for="user in userList" :key="user.id">{{ user.id }}</li>
        <li v-for="user in userList" :key="user.id">{{ user.name }}</li> -->

        <h1>Slot1</h1>
        <slot name="slotA" :text="text"></slot>

        <h2>Slot2</h2>
        <slot name="slotB"></slot>

        <h3>Slot3</h3>
        <slot name="slotC"></slot>
        
    </div>
</template>

<script setup lang="ts">
// import { PropType } from 'vue';


// interface User {
//     id: number,
//     name: string
// }

// defineProps ({
//     count: {
//         type: Number,
//         required: true,
//     },
//     test: {
//         type: Number,
//         default: 10
//     }, 
//     userList: {
//         type: Array as PropType<User[]>,
//         required: true
//     },

//     stringTittle: {
//         type: String,
//         default: "NHÌN Cái Gì"
//     },

// })
let text = "Xin chào"
</script>

<style scoped>

</style>