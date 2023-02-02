<template>
    <section class="pt-16">
        <AtomsContainer>
            <div class="flex justify-between pb-6">
                <div class="">
                    <AtomsTitle texte="Popular podcast"/>
                </div>
                <div class="flex items-center min-w-max gap-5">
                    <NuxtLink to="#">
                       See All
                    </NuxtLink>
                </div>
            </div>
            <div class="grid grid-cols-2 sm:grid-cols-3 lg:grid-cols-4 gap-x-3 gap-y-4 sm:gap-x-5 sm:gap-y-6">
                <!-- title, href, duration, coverImage, category, createdAt, description -->
                <CardsPodCast 
                    title="Start your journey in SEO" 
                    href="" 
                    duration="" 
                    cover-image="/images/podCast.jpg" 
                    category="" 
                    created-at="" 
                    description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae voluptates porro"
                />

                <CardsPodCast 
                    title="Start your journey in SEO" 
                    href="" 
                    duration="" 
                    cover-image="/images/podCast.jpg" 
                    category="" 
                    created-at="" 
                    description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae voluptates porro"
                />

                <CardsPodCast 
                    title="Start your journey in SEO" 
                    href="" 
                    duration="" 
                    cover-image="/images/podCast.jpg" 
                    category="" 
                    created-at="" 
                    description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae voluptates porro"
                />

                <CardsPodCast 
                    title="Start your journey in SEO" 
                    href="" 
                    duration="" 
                    cover-image="/images/podCast.jpg" 
                    category="" 
                    created-at="" 
                    description="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Recusandae voluptates porro"
                />

            </div>
        </AtomsContainer>
    </section>
</template>