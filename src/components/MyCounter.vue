<script setup>
import { ref } from 'vue';
const count = ref(0);
function increment () {
    count.value++
}
</script>
<template>
    <h3>MyCounter Component</h3>
    Reactive variable count: <b>{{ count }}</b>
    <br /><br />
    <button @click="increment">count+1</button>
</template>
<style scoped>
h1 {
    font-family: Arial, Helvetica, sans-serif;
    font-size: 20px;
}

.red-text {
    color: red;
}
</style>