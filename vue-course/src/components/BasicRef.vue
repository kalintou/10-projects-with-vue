<script setup>
import {onMounted, ref} from 'vue';
const myRef = ref('')
console.log(myRef.value)

onMounted(() => {
    console.log(myRef.value)
    myRef.value.focus()
    myRef.value.value = 'something else'
})
</script>


<template>
    <div>
        <input type="text" placeholder="Enter your name" ref="myRef">
    </div>
</template>
