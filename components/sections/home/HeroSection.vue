<template>
    <section class="relative w-full">
        <div class="absolute top-0 inset-x-0 h-64 flex items-start">
            <div
                class="h-24 w-2/3 bg-gradient-to-br from-primary opacity-20 blur-2xl dark:from-[#570cac] dark:invisible dark:opacity-40">
            </div>
            <div
                class="h-20 w-3/5 bg-gradient-to-r from-[#8cd66a] opacity-40 blur-2xl dark:from-[#670ccf] dark:opacity-40">
            </div>
        </div>
        <AtomsContainer class-name="relative">
            <div aria-hidden="true" class="absolute inset-y-0 w-44 left-0 hidden dark:flex">
                <div
                    class="h-full md:h-1/2 lg:h-full w-full bg-gradient-to-tr opacity-40 dark:blur-2xl dark:from-[#570cac] dark:opacity-20">
                </div>
            </div>
            <div
                class="grid lg:grid-cols-2 gap-10 xl:gap-14 relative pt-24 lg:max-w-none max-w-2xl md:max-w-3xl mx-auto">
                <div class="lg:py-6">
                    <div class="text-center lg:text-left">
                        <span class="px-2 py-1 rounded-md bg-gray-100 dark:bg-body text-primary ">New season
                            available</span>
                        <h1 class="text-gray-800 pt-4 dark:text-white font-bold text-4xl md:text-5xl lg:text-6xl">
                            Find and listen <br> Favorite <span
                                class="text-transparent bg-clip-text bg-gradient-to-br from-primary to-[#8cd66a]">Podcast</span>
                            on internet
                        </h1>
                    </div>

                    <p class="text-gray-600 dark:text-gray-300 pt-8 text-center lg:text-left mx-auto max-w-xl">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum, beatae omnis ipsa magnam neque
                        ut nam nesciunt esse fugit praesentium hic magni possimus illo consequatur.
                    </p>

                    <div class="flex items-center gap-3 pt-9 flex-col sm:flex-row sm:w-max sm:mx-auto lg:mx-0">
                        <AtomsLinkBtn href="#" variant="primary" class="w-full sm:w-max flex justify-center">
                            Join us
                        </AtomsLinkBtn>

                        <AtomsLinkBtn href="#" variant="costum" costum-span-class="px-6 md:px-7 hover:bg-primary/10"
                            costum-text-color="text-primary ">
                            <div class="flex items-center gap-3">
                                <span class="p-2 rounded-full border border-primary">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24"
                                        fill="currentColor" class="w-3 h-3">
                                        <path fill-rule="evenodd"
                                            d="M4.5 5.653c0-1.426 1.529-2.33 2.779-1.643l11.54 6.348c1.295.712 1.295 2.573 0 3.285L7.28 19.991c-1.25.687-2.779-.217-2.779-1.643V5.653z"
                                            clip-rule="evenodd" />
                                    </svg>
                                </span>

                                <span>
                                    Listening Episode
                                </span>
                            </div>
                        </AtomsLinkBtn>
                    </div>
                    <div class="pt-8 lg:pt-10 w-max mx-auto lg:mx-0">
                        <div class="flex items-center text-center flex-col sm:flex-row gap-4 sm:gap-0">
                            <div class="flex items-center">
                                <img src="/images/sidebiew.webp" width="40" alt="avatar"
                                    class="w-10 h-10 rounded-full border-2 border-white dark:border-gray-400 object-cover">
                                <img src="/images/sidebiew.webp" width="40" alt="avatar"
                                    class="w-10 h-10 rounded-full border-2 border-white dark:border-gray-400 object-cover -ml-2.5">
                                <img src="/images/sidebiew.webp" width="40" alt="avatar"
                                    class="w-10 h-10 rounded-full border-2 border-white dark:border-gray-400 object-cover -ml-2.5">
                                <img src="/images/sidebiew.webp" width="40" alt="avatar"
                                    class="w-10 h-10 rounded-full border-2 border-white dark:border-gray-400 object-cover -ml-2.5">
                                <span
                                    class="w-10 h-10 rounded-full border-2 border-white dark:border-gray-400 bg-body-color flex items-center justify-center text-xs text-gray-300 object-cover -ml-2.5">
                                    300+
                                </span>
                            </div>
                            <div class="pl-2 text-gray-600 dark:text-gray-200">
                                WordWide listners
                            </div>
                        </div>
                    </div>
                </div>
                <div class="lg:h-full  hidden md:flex">

                    <div
                        class="flex w-full h-96 min-h-[24rem] lg:min-h-[none] lg:w-full lg:h-full items-center relative">
                        <div
                            class="absolute z-0 top-1/2  -translate-y-1/2 w-5/6 right-0 h-[calc(80%+20px)] bg-gradient-to-tr opacity-25 from-primary to-pink-300 dark:from-[#570cac] dark:to-primary blur-2xl">
                        </div>
                        <div
                            class="absolute w-3/5 h-full z-10 p-1 -translate-y-1/2 top-1/2 right-3 rounded-3xl bg-white dark:bg-body shadow-lg shadow-box-shadow border border-box-border">
                            <img src="/images/sidebiew.webp" alt="In studio" width="500" height="auto" loading="lazy"
                                class="w-full h-full rounded-2xl object-cover">
                        </div>
                        <div
                            class="absolute  -translate-y-1/2 top-1/2 h-[calc(80%-2rem)] w-[calc(40%-20px)] p-1 rounded-3xl bg-white dark:bg-body shadow-lg shadow-box-shadow border border-box-border ">
                            <img src="/images/sidebiew.webp" alt="Happy in studio" width="200" height="auto"
                                loading="lazy" class="w-full h-full rounded-2xl object-cover">
                        </div>
                    </div>
                </div>
            </div>
        </AtomsContainer>
    </section>
</template>