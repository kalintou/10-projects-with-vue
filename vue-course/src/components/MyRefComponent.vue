<script setup>
import {ref} from 'vue'
let userInfo = ref({name: 'Alex', age: 20, location: ['NYC','IDK'], isMarried: false})
</script>

<template>

<h1>Name: {{ userInfo.name }}</h1>
<h1>Age: {{ userInfo.age }}</h1>
<h1>Location: {{ userInfo.location }}</h1>
<h1>isMarried: {{ userInfo.isMarried }}</h1>

<button @click="userInfo.name='HuXn'">Change Name</button>
<button @click="userInfo.age= 40">Change Age</button>
<button @click="userInfo.location= ['Earth', 'Minami']">Change Location</button>
<button @click="userInfo.isMarried= true">Change Status</button>

</template>