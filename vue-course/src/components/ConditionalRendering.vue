<script setup>

import {ref} from 'vue'

let password = ref(0)

</script>

<template>
    <h1 v-if="password.length > 8">Strong Password</h1>
    <h1 v-else-if="password.length < 8">Weak Password</h1>
    <h1 v-else>Please Enter Your Password</h1>
</template>