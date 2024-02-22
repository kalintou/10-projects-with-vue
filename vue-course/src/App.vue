<script setup>
import {provide} from 'vue'
import PracticeComponent from './components/PracticeComponent.vue';

provide('friends', ['kan' ,'jordan','HuXn','Jogn'])
provide('games', {
  id: 1,
  title: "Epic adad",
  genre: ['Action','Adventrue', 'RPG'],
  platform: ['Windows','Mac']
})

provide('moreGames', [
{
    title: 'Space 1',
    genre: 'SF',
    platform: 'PC',
    releaseDate: '1999'
  },
  {
    title: 'Space 2',
    genre: 'SFF',
    platform: 'PC',
    releaseDate: '1999'
  },
  {
    title: 'Space 3',
    genre: 'SFFF',
    platform: 'PC',
    releaseDate: '1999'
  },
  {
    title: 'Space 3',
    genre: 'SFFF',
    platform: 'PC',
    releaseDate: '1999'
  }
])

</script>




<template>

  <PracticeComponent />

</template>
