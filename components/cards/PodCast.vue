<template>
    <div
        class="lg:p-1 relative h-auto flex flex-col lg:rounded-2xl lg:bg-box-bg lg:shadow-lg lg:shadow-box-shadow lg:border lg:border-box-border">
        <div class="relative h-max min-h-max">
            <img :src="coverImage" alt="Cover image" width="280"
                class="w-full h-32 sm:h-36 md:h-40 lg:h-48 rounded-xl object-cover">
                <span class="absolute top-2 right-2 px-2 rounded-full text-sm text-white bg-primary">
            {{ duration }}
        </span>
        </div>
        <div class="lg:px-2 pt-2 lg:pb-4 xl:px-4 md:pt-4  h-full flex flex-col justify-between">
            <div class="h-full">
                <h2 class="font-semibold text-base md:text-lg lg:text-xl line-clamp-2 md:line-clamp-3 text-gray-700 dark:text-white">
                    {{ title }}
                </h2>
            </div>
            <div class="pt-3 sm:pt-5 min-h-max h-max">
                <NuxtLink :to="href"
                    class="flex relative group items-center text-white px-5 py-2 bg-primary gap-1 text-sm w-max rounded-full">
                    <span class="absolute inset-0 rounded-full group-hover:scale-105 origin-center transition-all ease-in-out bg-primary">

                    </span>
                    <span class="relative flex items-center gap-3">
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24"
                            fill="currentColor" class="w-3 h-3">
                            <path fill-rule="evenodd"
                                d="M4.5 5.653c0-1.426 1.529-2.33 2.779-1.643l11.54 6.348c1.295.712 1.295 2.573 0 3.285L7.28 19.991c-1.25.687-2.779-.217-2.779-1.643V5.653z"
                                clip-rule="evenodd" />
                        </svg>
                    Play now
                    </span>
                </NuxtLink>
            </div>
        </div>
    </div>
</template>
<script lang="ts" setup>
const { title, href, duration, coverImage, category, createdAt, description } = defineProps<{
    title: string,
    href: string,
    duration: string,
    coverImage: string,
    category: string,
    createdAt: string,
    description: string
}>()
</script>