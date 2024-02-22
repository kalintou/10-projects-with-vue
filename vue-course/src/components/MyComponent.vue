<script setup>
const vFormateDiv = {
    mounted: (el, binding) => {
        switch (binding.arg) {
            case 'orange':
                el.style.color = 'orange'
                break;
            case 'pink':
                el.style.color = 'pink'
                break;
            case 'purple':
                el.style.color = 'purple'
                break;
            case 'teal':
                el.style.color = 'teal'
                break;
            default:
                el.style.color = 'black'
        }
    }
}
</script>

<template>
    <div v-formate-div:orange>Using simple custom directive</div>
    <div v-formate-div:pink>Using simple custom directive</div>
    <div v-formate-div:purple>Using simple custom directive</div>
    <div v-formate-div:teal>Using simple custom directive</div>
</template>
