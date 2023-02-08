<template>
    <footer class="pt-20 bg-gray-100 dark:bg-body border-t border-gray-200 dark:border-gray-100/20">
        <AtomsContainer class-name="pb-10">
            <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-8 gap-y-10">
                <div class="col-span-2 md:col-span-4 lg:col-span-2">
                    <NuxtLink to="/" class=" flex items-center gap-2">
                        <span class="flex">
                            <span class="w-3 h-6 rounded-l-full flex bg-primary"></span>
                            <span class="w-3 h-6 rounded-r-full flex bg-[#f88fc2] mt-2"></span>
                        </span>
                        <span class="text-xl font-bold text-gray-700 dark:text-white">Podux</span>
                    </NuxtLink>

                    <p class="text-gray-600 dark:text-gray-300 pt-6">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Officia nemo, veritatis
                    </p>
                </div>

                <BlocksFooterNavBlock title="Enterprise" :links="quickLinks" />
                <BlocksFooterNavBlock title="Ressources" :links="ressourcesLinks" />
                <BlocksFooterNavBlock title="Support" :links="supportLinks" />
                <BlocksFooterNavBlock title="Enterprise" :links="quickLinks" />
            </div>
        </AtomsContainer>
        <div class="py-2 bg-gray-200 dark:bg-[rgb(10,16,29)]">
            <AtomsContainer>
                <div class="flex justify-between items-center gap-5 text-gray-600 dark:text-gray-300">
                    <div class="">
                        &copy; {{ new Date().getFullYear() }} Allright Reserved. Designed by <NuxtLink target="_blank"
                            to="#" class="font-bold text-primary">Kat Mj</NuxtLink>
                    </div>

                    <div class="flex items-center gap-x-3">
                        <NuxtLink target="_blank" to="#" class="transition hover:!text-primary">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor"
                                class="w-5 h-5" viewBox="0 0 16 16">
                                <path
                                    d="M5.026 15c6.038 0 9.341-5.003 9.341-9.334 0-.14 0-.282-.006-.422A6.685 6.685 0 0 0 16 3.542a6.658 6.658 0 0 1-1.889.518 3.301 3.301 0 0 0 1.447-1.817 6.533 6.533 0 0 1-2.087.793A3.286 3.286 0 0 0 7.875 6.03a9.325 9.325 0 0 1-6.767-3.429 3.289 3.289 0 0 0 1.018 4.382A3.323 3.323 0 0 1 .64 6.575v.045a3.288 3.288 0 0 0 2.632 3.218 3.203 3.203 0 0 1-.865.115 3.23 3.23 0 0 1-.614-.057 3.283 3.283 0 0 0 3.067 2.277A6.588 6.588 0 0 1 .78 13.58a6.32 6.32 0 0 1-.78-.045A9.344 9.344 0 0 0 5.026 15z">
                                </path>
                            </svg>
                        </NuxtLink>

                        <NuxtLink target="_blank" to="https://github.com/johnkat-mj" class="transition hover:!text-primary">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor"
                                class="w-5 h-5" viewBox="0 0 16 16">
                                <path
                                    d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z">
                                </path>
                            </svg>
                        </NuxtLink>
                    </div>
                </div>
            </AtomsContainer>
        </div>
    </footer>
</template>

<script lang="ts" setup>
const quickLinks = [
    {
        href: "#",
        text: "About us"
    },
    {
        href: "#",
        text: "News"
    },
    {
        href: "#",
        text: "Team"
    },
    {
        href: "#",
        text: "Solution"
    }
]
const ressourcesLinks = [
    {
        href: "#",
        text: "Developpers"
    },
    {
        href: "#",
        text: "Integration"
    },
    {
        href: "#",
        text: "Pricing"
    }
]

const supportLinks = [
    {
        href: "#",
        text: "Contact-us"
    },
    {
        href: "#",
        text: "Licence"
    },
    {
        href: "#",
        text: "Terms"
    },
    {
        href: "#",
        text: "FAQ"
    }
]


</script>