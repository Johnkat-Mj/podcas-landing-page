<template>
    <section class="pt-16 relative">
        <div aria-hidden="true" class="absolute inset-y-0 w-44 left-0 hidden dark:flex">
            <div
                class="h-full md:h-1/2 lg:h-full w-full bg-gradient-to-tr opacity-40 dark:blur-2xl dark:from-[#570cac] dark:opacity-20">
            </div>
        </div>
        <div class="absolute top-14 inset-x-0 h-64 flex items-start">
            <div
                class="h-24 w-2/3 bg-gradient-to-br from-primary opacity-20 blur-2xl dark:from-[#570cac] dark:invisible dark:opacity-40">
            </div>
            <div
                class="h-20 w-3/5 bg-gradient-to-r from-[#8cd66a] opacity-40 blur-2xl dark:from-[#670ccf] dark:opacity-40">
            </div>
        </div>
        <AtomsContainer class-name="relative">
            <div class="flex justify-between pb-6 relative">
                <div class="">
                    <AtomsTitle texte="Popular podcast" />
                </div>
                <div class="flex items-center min-w-max gap-5">
                    <AtomsLinkBtn href="#" variant="primary">
                        See all
                    </AtomsLinkBtn>
                </div>
            </div>
            <div
                class="grid grid-cols-2 items-stretch sm:grid-cols-3 lg:grid-cols-4 gap-x-3 gap-y-10 sm:gap-x-5 sm:gap-y-8">
                <!-- title, href, duration, coverImage, category, createdAt, description -->
                <CardsPodCast title="Start your journey in SEO" href="#" duration="24min" cover-image="/images/podCast.jpg"
                    category="" created-at="" description="Lorem ipsum dolor sit amet,  voluptates porro" />

                <CardsPodCast title="Start your journey in SEO" href="#" duration="24min" cover-image="/images/podCast.jpg"
                    category="" created-at=""
                    description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae voluptates porro" />

                <CardsPodCast title="Start your journey in SEO" href="#" duration="24min" cover-image="/images/podCast.jpg"
                    category="" created-at=""
                    description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae voluptates porro" />

                <CardsPodCast title="Start your journey in SEO" href="#" duration="24min" cover-image="/images/podCast.jpg"
                    category="" created-at=""
                    description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae voluptates porro" />

            </div>
        </AtomsContainer>
    </section>
</template>