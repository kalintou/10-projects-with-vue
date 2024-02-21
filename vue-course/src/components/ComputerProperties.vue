<script setup>
import {ref, computed} from 'vue'

const counter = ref(0)

const squaredCounter = computed(() => counter.value ** 2)

const incrementCounter = () => {
    counter.value++
}

</script>

<template>
    <h1>Counter: {{ counter }}</h1>
    <p>Squared Counter: {{ squaredCounter }}</p>
    <button @click="incrementCounter">Increment Counter</button>

</template>