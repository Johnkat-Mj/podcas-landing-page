<script lang="ts" setup>
    const { text, href } = defineProps<
    {
        text:string,
        href:string
    }>()
</script>
<template>
    <li class="lg:inline-flex">
        <NuxtLink class="lg:inline-flex transition hover:text-primary ease-linear text-lg" :to="href">
            {{ text }}
        </NuxtLink>
    </li>
</template>