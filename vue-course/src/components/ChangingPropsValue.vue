<script setup>
const myFavoriteNumberProp = defineProps(['myFavoriteNumber'])

</script>

<template>
    <h1>{{ myFavoriteNumberProp.myFavoriteNumber }}</h1>
</template>