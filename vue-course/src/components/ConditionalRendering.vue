<script setup>

const isTrue = false;
const isFalse = false;

</script>

<template>
    <div>
        <p v-if="isTrue">This will how if isTrue is true</p>
        <p v-else-if="isFalse">This will how if isFalse is true</p>
        <p v-else>Both false</p>
    </div>
</template>