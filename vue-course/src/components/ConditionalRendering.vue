<script setup>

import {ref} from 'vue'
let isVisible = ref(false)

</script>

<template>
    <p v-show="isVisible">This paragraph will be shown or hidden based on the value of isVisible</p>
    <button @click="isVisible=true">show</button>
    <button @click="isVisible=false">close</button>
</template>