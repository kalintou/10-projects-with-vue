<script setup>

import LifeCycleComponent from './components/LifeCycleComponent.vue';
import {ref} from 'vue'
const showHide = ref(true)
</script>

<template>

  <LifeCycleComponent v-if="showHide" />
  <button @click="showHide = !showHide">show / Hide</button>

</template>
