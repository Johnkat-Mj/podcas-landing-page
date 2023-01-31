<template>
    <section class="relative w-full">
        <div class="absolute top-0 inset-x-0 h-32">
            <div class="w-3/5 h-24 bg-gradient-to-b from-primary blur-xl flex"></div>
        </div>
        <AtomsContainer>
            <div class="grid lg:grid-cols-2 lg:gap-14 relative">
                <div class="">
                    <div>
                        <span class="text-primary">New season available</span>
                        <h1 class="text-gray-800 dark:text-white font-bold uppercase text-4xl md:text-5xl lg:text-6xl">
                            LIVE decoders <br> are <span
                                class="text-transparent bg-clip-text bg-gradient-to-br from-primary to-[#8cd66a]">what</span>
                            we do
                        </h1>
                    </div>
                    <p class="text-gray-600 dark:text-gray-300 pt-8">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum, beatae omnis ipsa magnam neque
                        ut nam nesciunt esse fugit praesentium hic magni possimus illo consequatur.
                    </p>

                    <div class="flex items-center gap-3 pt-9 flex-col sm:flex-row">
                        <AtomsLinkBtn href="#" variant="primary">
                            Join us
                        </AtomsLinkBtn>

                        <AtomsLinkBtn href="#" variant="costum" costum-span-class="px-6 md:px-7 hover:bg-primary/10"
                            costum-text-color="text-primary ">
                            <div class="flex items-center gap-3">
                                <span class="p-2 rounded-full border border-primary">
                                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"
                                    class="w-3 h-3">
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
                    <div class="pt-8 lg:pt-10">
                        <div class="flex items-center">
                            
                        </div>
                    </div>
                </div>
                <div class="">
                    <div class="w-2/5 aspect-square rounded-full border-4 border-box-border"></div>
                </div>
            </div>
        </AtomsContainer>
    </section>
</template>