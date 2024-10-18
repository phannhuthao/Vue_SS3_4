<template>
    <div class="sex">
        <p>Giới Tính: {{ gender }} </p>
        <br>
        <input v-model="gender" type="radio" value="Nam">Nam</input>
        <br>
        <input v-model="gender" type="radio" value="Nữ" >Nữ</input>
        <br>
        <input v-model="gender" type="radio" value="Khác">Khác</input>

    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

let gender = ref('');
</script>

<style scoped>
.sex {
    text-align: center;
    border: 10px;
}
</style>