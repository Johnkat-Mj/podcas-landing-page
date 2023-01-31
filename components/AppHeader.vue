<script lang="ts" setup>
const navLinks=[
    {
        text:"Podcast",
        href:"/"
    },
    {
        text:"Solution",
        href:"/"
    },
    {
        text:"Blog",
        href:"/"
    },
    {
        text:"About",
        href:"/"
    }
]
</script>
<template>
    <header class="absolute inset-x-0 top-0 py-3 z-50">
        <AtomsContainer>
            <nav class="flex items-center justify-between w-full">
                <!-- app logo -->
                <div class="inline-flex">
                    <NuxtLink to="/" class=" flex items-center gap-2">
                        <span class="flex">
                            <span class="w-3 h-6 rounded-l-full flex bg-primary"></span>
                            <span class="w-3 h-6 rounded-r-full flex bg-[#f88fc2] mt-2"></span>
                        </span>
                        <span class="text-lg text-gray-700 dark:text-white">Podux</span>
                    </NuxtLink>
                </div>
                <div class="flex">
                    <ul class="text-gray-700 dark:text-gray-100 flex items-center gap-8">
                        <AtomsNavLink v-for="navItem in navLinks" :href="navItem.href" :text="navItem.text"/>
                    </ul>
                </div>
                <div class="flex items-center bg-inherit gap-3 min-w-max">
                    <ElementsThemeSwitcher/>
                    <AtomsLinkBtn href="" variant="primary">
                        Join Us
                    </AtomsLinkBtn>
                </div>
            </nav>
        </AtomsContainer>
    </header>
</template>