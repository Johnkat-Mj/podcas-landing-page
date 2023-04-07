<template>
    <section class="pt-20 md:pt-24">
        <AtomsContainer>
            <div class="grid md:grid-cols-2 gap-10 xl:gap-14 relative">
                <div class="md:py-2 lg:py-4 relative">
                    <div class="absolute left-0 top-0 h-full w-full flex justify-end">
                        <span class="flex opacity-20">
                            <span class="w-16 h-32 rounded-l-full flex bg-primary blur-2xl"></span>
                            <span class="w-16 h-32 rounded-r-full flex bg-[#f88fc2] blur-2xl mt-14"></span>
                        </span>
                    </div>
                    <div class="relative">
                        <AtomsTitle texte="Find out what makes up different from others" />
                        <p class="text-gray-600 dark:text-gray-300 pt-8">
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Alias labore quas natus?
                            Repudiandae tempora autem corporis voluptatem ipsam voluptatibus
                        </p>
                        <div class="space-y-4 pt-8">
                            <div class="p-4 rounded-xl border border-box-border transition hover:bg-gray-200 dark:hover:bg-box-bg">
                                <h3 class="text-gray-700 dark:text-gray-200 font-semibold text-xl">Last and feasible topics</h3>
                                <p class="text-base text-gray-600 dark:text-gray-300">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                            </div>
                            <div class="p-4 rounded-xl border border-box-border transition hover:bg-gray-200 dark:hover:bg-box-bg">
                                <h3 class="text-gray-700 dark:text-gray-200 font-semibold text-xl">Last and feasible topics</h3>
                                <p class="text-base text-gray-600 dark:text-gray-300">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                            </div>
                            <div class="p-4 rounded-xl border border-box-border transition hover:bg-gray-200 dark:hover:bg-box-bg">
                                <h3 class="text-gray-700 dark:text-gray-200 font-semibold text-xl">Last and feasible topics</h3>
                                <p class="text-base text-gray-600 dark:text-gray-300">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                            </div>
                        </div>
                        <div class="pt-10 flex">
                            <AtomsLinkBtn href="#" variant="primary">
                                Start Listning
                            </AtomsLinkBtn>
                        </div>
                    </div>
                </div>
                <div class="flex md:h-full relative">
                    <div
                            class="absolute z-0 top-1/2  -translate-y-1/2 w-5/6 right-0 h-[calc(80%+20px)] bg-gradient-to-tr opacity-25 from-primary to-pink-300 dark:from-[#570cac] dark:to-primary blur-2xl">
                        </div>
                    <div
                        class="w-full h-[27rem] sm:h-[30rem] md:h-full flex justify-start md:justify-end relative pb-5">
                        <img src="/images/podCast.webp" alt="Podcast image" width="300" class="w-2/5 aspect-square absolute bottom-0 right-0 md:left-0 object-cover  rounded-t-[30%] rounded-b-[30%] border-4 border-box-border shadow-md shadow-box-shadow">
                        <img src="/images/concentrated-young-african-american.webp" alt="Illustratuin about" width="500"
                            class="w-11/12 lg:w-5/6 h-full object-cover rounded-t-[10rem] rounded-b-[10rem] md:rounded-t-[11rem] md:rounded-b-[11rem] lg:rounded-t-[14rem] lg:rounded-b-[14rem]">
                    </div>
                </div>
            </div>
        </AtomsContainer>
    </section>
</template>