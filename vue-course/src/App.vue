<script setup>

import SlotComponent from './components/SlotComponent.vue';
import FallbackContent from './components/FallbackContent.vue'
</script>


<template>
  <SlotComponent>
    <h1>Content 1</h1>
    <h2>Content 2</h2>
  </SlotComponent>

  <hr>

  <FallbackContent>

  </FallbackContent>

  <FallbackContent>
    <p>Fallback will not work becuase ....</p>
  </FallbackContent>
</template>
