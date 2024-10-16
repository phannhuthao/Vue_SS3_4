<template>
    <div>
        <button 
            :class="{ active: activeIndex === 1 }" 
            @click="setActiveIndex(1)">
            Button 1
        </button>
        <button 
            :class="{ active: activeIndex === 2 }" 
            @click="setActiveIndex(2)">
            Button 2
        </button>
        <button 
            :class="{ active: activeIndex === 3 }" 
            @click="setActiveIndex(3)">
            Button 3
        </button>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

let activeIndex = ref(1);

const setActiveIndex = (index: number) => {
    activeIndex.value = index;
}
</script>

<style scoped>
button {
    margin: 5px;
    padding: 10px;
    font-size: 16px;
}

button.active {
    background-color: red;
    color: #fff;
}
</style>
