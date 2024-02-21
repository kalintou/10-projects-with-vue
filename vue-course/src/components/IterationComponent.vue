<script setup>

import {ref} from 'vue'

const movies = ref([
    ['movie1','movie2','movie3','movie4','movie5'],
    ['movie6','movie7','movie8','movie9','movie10'],
    ['movie11','movie12','movie13','movie14','movie15'],
    ['movie16','movie17','movie18','movie19','movie20'],
])
</script>

<template>
    <ul v-for="(movie, i) in movies" :key="i">
        <li v-for="(m, index) in movie" :key="index">{{ m }}</li>
    </ul>
</template>