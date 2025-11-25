<script setup>
import { ref, computed } from 'vue';

// usage of ref() to create a reactive variable
const count = ref(0);

// usage of computed() to create a computed property
const doubleCount = computed(() => count.value * 2);

function increment () {
    count.value++
}
</script>
<template>
    <h3>MyCounter Component</h3>
    Reactive variable count: <b>{{ count }}</b>
    <br /><br />
    Computed property doubleCount: <b>{{ doubleCount }}</b>
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