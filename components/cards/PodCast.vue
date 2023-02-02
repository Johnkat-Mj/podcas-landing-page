<template>
    <div class="sm:p-1 h-auto rounded-2xl sm:bg-body sm:shadow-lg sm:shadow-box-shadow sm:border sm:border-box-border">
        <div class="relative h-max min-h-max">
            <img :src="coverImage" alt="Cover image" width="280" class="w-full h-32 sm:h-36 md:h-40 rounded-xl object-cover">
        </div>
        <div class="sm:px-2 pt-2 pb-4 md:px-4 md:pt-4 md:pb-5">
            <h2 class="font-semibold text-base md:text-lg line-clamp-2 text-gray-700 dark:text-white">
                {{ title }}
            </h2>
            <p class="text-gray-600 dark:text-gray-300 !hidden sm:!flex sm:text-sm pt-2 md:pt-4 line-clamp-2 overflow-hidden">
                {{ description }}
            </p>
            <div class="pt-5">
                <NuxtLink :to="href" class="flex items-center text-white rounded-full p-0.5 pr-2 gap-1 text-sm border w-max">
                    <span class="p-1 rounded-full bg-primary">
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24"
                            fill="currentColor" class="w-3 h-3">
                            <path fill-rule="evenodd"
                                d="M4.5 5.653c0-1.426 1.529-2.33 2.779-1.643l11.54 6.348c1.295.712 1.295 2.573 0 3.285L7.28 19.991c-1.25.687-2.779-.217-2.779-1.643V5.653z"
                                clip-rule="evenodd" />
                        </svg>
                    </span>
                    Play now
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
    category:string,
    createdAt:string,
    description:string
}>()
</script>