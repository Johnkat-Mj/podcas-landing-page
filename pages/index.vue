<script setup lang="ts">
const colorMode = useColorMode()
console.log(colorMode.preference)
</script>
<template>
    <div>
        <SectionsHomeHeroSection/>
        <SectionsHomeLatestPodcast/>
        <SectionsHomePopularPodcasts/>

    </div>
</template>