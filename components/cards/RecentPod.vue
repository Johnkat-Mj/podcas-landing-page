<template>
    <div class="w-full relative rounded-2xl overflow-hidden">
        <nuxt-img :src="coverImage" alt="Cover image" width="2280" class="w-full aspect-square object-cover rounded-2xl" />
        <span class="absolute top-2 right-2 px-2 rounded-full text-sm text-white bg-primary">
            {{ duration }}
        </span>
        <div
            class="absolute py-2 px-3 md:py-3 md:px-4 bottom-0 h-28 flex flex-col justify-between inset-x-0 bg-gradient-to-t from-gray-800 bg-opacity-50 backdrop-filter backdrop-blur-sm">
            <h2 class="text-white font-semibold text-sm sm:text-base line-clamp-2">
                {{ title }}
            </h2>
            <div class="pt-2">
                <NuxtLink :to="href"
                    class="flex items-center text-white rounded-full p-0.5 pr-2 gap-2 text-sm border border-gray-100/20 w-max">
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
const { title, href, duration, coverImage } = defineProps<{
    title: string,
    href: string,
    duration: string,
    coverImage: string
}>()
</script>