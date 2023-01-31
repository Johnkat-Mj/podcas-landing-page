<script lang="ts" setup>
const { className } = defineProps<{className?:string}>()
</script>
<template>
    <div class="w-full px-5 sm:px-8 md:px-12 lg:px-8 max-w-screen-lg lg:max-w-screen-xl mx-auto " :class="{ className }">
        <slot/>
    </div>
</template>