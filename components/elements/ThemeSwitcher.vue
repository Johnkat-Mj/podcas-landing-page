<script lang="ts" setup>
const isOpen = useState("isOpen", ()=>false)
function changeTheme(event:MouseEvent){
    event.preventDefault()
    isOpen.value = !isOpen.value
}
</script>
<template>
    <div class="relative py-2">
        <button class="outline-none bg-body p-2.5 rounded-full text-gray-600 dark:text-gray-300 hover:bg-gray-100 dark:hover:bg-gray-800" @click="(event)=>{
            changeTheme(event)
        }">
            <ElementsIconsSystem v-if="$colorMode.preference === 'system'" />
            <ElementsIconsLight v-if="$colorMode.preference === 'light'" />
            <ElementsIconsDark v-if="$colorMode.preference === 'dark'" />
        </button>
        <div v-if="isOpen" class="fixed inset-0 z-30 bg-red-500" @click="isOpen = false"></div>
        <transition 
            enter-active-class="ease-out duration-300"
            enter-from-class="transition transform opacity-0 translate-y-6"
            enter-to-class="transition transform opacity-100 translate-y-0"
            leave-active-class="transition ease-in duration-200" 
            leave-from-class="transform opacity-100 translate-y-0"
            leave-to-class="transform opacity-0 translate-y-6">
            <div v-show="isOpen" class="absolute border border-box-border shadow-md shadow-box-shadow z-40 top-full right-0 transition-all ease-linear p-2 rounded-xl w-44 bg-box-bg">
                <ul class="flex flex-col" @click="isOpen = false">
                    <li
                        class="flex select-none cursor-pointer items-center gap-3 px-2 py-2 rounded-md transition hover:bg-gray-100 dark:hover:bg-gray-800 text-gray-600 dark:text-gray-200" @click="$colorMode.preference = 'system'">
                        <span>
                            <ElementsIconsSystem />
                        </span>
                        <span>
                            System
                        </span>
                    </li>

                    <li
                        class="flex select-none cursor-pointer items-center gap-3 px-2 py-2 rounded-md transition hover:bg-gray-100 dark:hover:bg-gray-800 text-gray-600 dark:text-gray-200" @click="$colorMode.preference = 'light'">
                        <span>
                            <ElementsIconsLight />
                        </span>
                        <span>
                            Light
                        </span>
                    </li>

                    <li
                        class="flex select-none cursor-pointer items-center gap-3 px-2 py-2 rounded-md transition hover:bg-gray-100 dark:hover:bg-gray-800 text-gray-600 dark:text-gray-200" @click="$colorMode.preference = 'dark'">
                        <span>
                            <ElementsIconsDark />
                        </span>
                        <span>
                            Dark
                        </span>
                    </li>
                </ul>
            </div>
        </transition>

    </div>
</template>
