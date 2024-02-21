<script setup>
import {reactive,ref} from 'vue'
let initialState = reactive({val: {count: 0}, user: ['Huxu', 'Kan']})

const changeUser = () => {
    initialState.user[0] = 'Michel'
    initialState.user[1] = 'fawe'
}
</script>

<template>
    <h1>Current Count: {{ initialState.val.count }}</h1>
    <h2>Users: {{ initialState.user }}</h2>
    <button @:click="initialState.val.count += 10">Add 10</button>
    <button @:click="changeUser">Change User</button>
    <button @:click="initialState.user.push('John fwea')">Add One More</button>
</template>