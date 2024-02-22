<script setup>
import {inject} from 'vue'
const friendsList = inject('friends')
const games = inject('games')
const moreGames = inject('moreGames')


</script>


<template>
<h1>Injecting Array</h1>
<ul v-for="(friend, index) in friendsList" :key="index">
    <li>{{ friend }}</li>
</ul>

<hr>

<ul v-for="(game, index) in games" :key="index">
    <li>{{ game }}</li>
</ul>

<hr>

<ul v-for="(moreGame, index) in moreGames" :key="index">
    <li>{{ moreGame }}</li>
</ul>
</template>
