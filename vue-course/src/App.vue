<script setup>

import SchoolComponent from './components/SchoolComponent.vue';
import {provide} from 'vue';

provide('studentName', 'Alex')
provide('studentAge', 20)
provide('studentLocation', ['China','Shanghai'])

// const studentName = 'alex'
// const studentAge = 20
// const studentLocation = ['China', 'Shanghai']

</script>


<template>

  <SchoolComponent />

</template>
