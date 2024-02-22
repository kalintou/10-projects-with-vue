<script setup>
import {ref, watch} from 'vue'
const username = ref('jordan')
const count = ref(0)

watch([username, count], (newVal, oldVal) => {
    console.log('New Value', newVal)
    console.log('Old Value', oldVal)
}) 
</script>


<template>
    <h1>{{ username }}</h1>
    <h1>Count: {{ count }}</h1>
    
    <button @click="username = 'Kan'">Change Name</button>
    <button @click="count++">Increment Counter</button>
</template>
