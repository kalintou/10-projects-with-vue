<script setup>

import {
    ref,
    onBeforeMount,
    onMounted,
    onBeforeUpdate,
    onUpdated,
    onBeforeUnmount,
    onUnmounted
} from 'vue'

const message = ref('Hello Vue!')

onBeforeMount(() => {
    console.log('Component is about to be mounted')
})

onMounted(() => {
    console.log('Component has been mounted')
}) 

onBeforeUpdate(() => {
    console.log('Component is about to update')
})

onUnmounted(() => {
    console.log('Component has been unmounted')
})

const updateMessage = () => {
    message.value = 'Updated Message!'
}

onBeforeUnmount(() => {
    console.log('Component is about to be unmounted')
})

onUpdated(() => {
    console.log('Component has been updated')
})

</script>


<template>
    <p>{{ message }}</p>
    <button @click="updateMessage">Update Message</button>
</template>
