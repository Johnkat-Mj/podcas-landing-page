
<template>
    <h2 class="text-2xl md:text-3xl text-gray-800 dark:text-white font-bold">
        {{ texte }}
    </h2>
</template>
<script lang="ts" setup>
const { texte } = defineProps<{texte:string}>()
</script>