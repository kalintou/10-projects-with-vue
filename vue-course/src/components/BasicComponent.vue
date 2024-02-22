<script setup>
import {ref, watch} from 'vue'
//import { compileScript } from 'vue/compiler-sfc';
const message = ref('Hello, Vue!')
const inputText = ref('')

//watch for changes in inputText and update message accordingly
watch(inputText, (newValue, oldValue) => {
    //You can perform some logic here when inputText Chnages.
    console.log(newValue)
    console.log(oldValue)
    message.value = `You typed: ${newValue}`
})

</script>


<template>
    <div>
        <h1>{{ message }}</h1>
        <input v-model="inputText" placeholder="Type Something...">
    </div>
</template>
