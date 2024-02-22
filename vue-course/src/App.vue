<script setup>

import NamedSlot from './components/NamedSlot.vue'

</script>


<template>

  <NamedSlot>
    <template #one>
      <h1>one</h1>
    </template>
    <template #two>
      <h1>two</h1>
    </template>
  </NamedSlot>

</template>
