<template>
    <div id="userComponent">
        <img
            @click="openMenu = !openMenu"
            data-tooltip-target="tooltip-no-arrow-user"
            data-tooltip-placement="bottom"
            src="https://placehold.co/40"
            class="rounded-full w-8 cursor-pointer">

            <div 
                v-show="!openMenu"
                id="tooltip-no-arrow-user"
                role="tooltip"
                class="
                    inline-block 
                    absolute 
                    invisible 
                    text-xs 
                    z-10 
                    py-1 
                    px-2 
                    font-medium 
                    text-white 
                    rounded-sm 
                    shadow-sm 
                    opacity-0 
                    tooltip 
                    bg-gray-600
                    delay-150
                "
                >
                <div>Google Account</div>
                <div class="text-gray-300">
                    John Doe
                </div>
                <div class="text-gray-300">
                    john.doe@gmail.com
                </div>
            </div>

            <div 
                v-show="openMenu"
                class="
                    absolute 
                    z-10
                    w-80
                    right-2
                    bg-white
                    top-14
                    rounded-lg
                    "
                >

                <div class="w-full flex justify-center">
                    <img
                    src="https://placehold.co/70"
                    class="rounded-full w-20 mt-4" />
                </div>
                <div class="text-gray-700 w-full flex justify-center mt-2 text-lg">
                    John Doe
                </div>
                <div class="text-gray-700 w-full flex justify-center mt-2 text-sm pb-4 border-b">
                    john.doe@mail.com
                </div>
                <div class="flex justify-center my-5">
                    <button class="
                        bg-transparent
                        text-xs
                        hover:bg-gray-100
                        text-gray-600
                        font-semibold
                        py-2
                        px-4
                        border
                        border-gray-300
                        rounded
                        "   >
                        Sign out of Gmail
                    </button>
                </div>
            </div>
    </div>
</template>

<script setup>
import {ref} from 'vue';

let openMenu = ref(false);
</script>