<template>
    <h1 :class="$style['m-class']">Using Module CSS with $ syntax (habak-case)</h1>
</template>

<style module>
/* kabab-case */
.m-class {
    background: firebrick;
    color: white;
}
</style>