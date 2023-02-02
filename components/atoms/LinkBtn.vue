<script lang="ts" setup>
const { href, variant, costumSpanClass="", costumTextColor="" } = defineProps<{
    href:string,
    variant:"primary"|"primary-outlined"|"secondary"|"secondary-outlined"|"costum",
    costumSpanClass?:string,
    costumTextColor?:string
}>()

let spanClass:string = "";
let textCl:string = ""
if (variant === "primary") {
    spanClass = "bg-primary border-2 border-transparent"
    textCl = "text-white"
}else if(variant === "primary-outlined"){
    spanClass = "border-2 border-primary"
    textCl = "text-primary"
}
else if(variant === "secondary"){
    spanClass = "bg-primary/5"
    textCl = "text-primary"
}
else if(variant === "costum"){
    spanClass=costumSpanClass
    textCl = costumTextColor
}

</script>
<template>
    <NuxtLink :to="href" class="px-6 md:px-7 py-3 rounded-full relative group">
        <span v-if="variant!=='costum'" class="absolute inset-0 rounded-full group-hover:scale-105 origin-center transition-all ease-in-out" :class="spanClass"></span>
        <span class="relative flex items-center justify-center" :class="textCl">
            <slot/>
        </span>
    </NuxtLink>
</template>