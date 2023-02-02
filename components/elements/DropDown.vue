<script lang="ts" setup>
const isOpenDrop = useState("isOpenDrop", () => false)
function changeTheme(event: MouseEvent) {
    event.preventDefault()
    isOpenDrop.value = !isOpenDrop.value
}
</script>
<template>
    <div class="relative py-2">
        <div
            class="bg-transparent"
            @click="(event) => {
                changeTheme(event)
            }">
            <slot name="trigger"/>
        </div>
        <div v-if="isOpenDrop" class="fixed inset-0 z-30" @click="isOpenDrop = false"></div>
        <transition enter-active-class="ease-out duration-300"
            enter-from-class="transition transform opacity-0 translate-y-6"
            enter-to-class="transition transform opacity-100 translate-y-0"
            leave-active-class="transition ease-in duration-200" leave-from-class="transform opacity-100 translate-y-0"
            leave-to-class="transform opacity-0 translate-y-6">
            <div v-show="isOpenDrop" @click="isOpenDrop = false"
                class="absolute border border-box-border shadow-md shadow-box-shadow z-40 top-full right-0 transition-all ease-linear p-2 rounded-xl w-44 bg-box-bg">
                <slot name="content"/>
            </div>
        </transition>
    </div>
</template>
