<script setup>

import {ref} from 'vue'

const books = ref([
    {
        id: 1,
        title: '1983',
        author: 'George Orwell',
        genre: 'Dystopian',
        publicationYear: 1949
    },
    {
        id: 2,
        title: '1984',
        author: 'George OOrwell',
        genre: 'SF',
        publicationYear: 1942
    },
    {
        id: 3,
        title: '1985',
        author: 'George OOOrwell',
        genre: 'SF',
        publicationYear: 1967
    },
    {
        id: 4,
        title: '1999',
        author: 'George OOOOrwell',
        genre: 'SF',
        publicationYear: 1267
    }
])

</script>

<template>
    <ul v-for="(book, index) in books" :key="index">
        <li>ID: {{ book.id }}</li>
        <li>Title: {{ book.title }}</li>
        <li>Author: {{ book.author }}</li>
        <li>Genre: {{ book.genre }}</li>
        <li>PublicationYear: {{ book.publicationYear }}</li>
    </ul>
</template>