<template>
    <header class="fixed top-0 left-0 right-0 dark:bg-black z-10 bg-gray-100">
        <nav class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8" aria-label="Global">
            <div class="flex lg:flex-1">
                <a href="#" class="-m-1.5 p-1.5">
                    <span class="sr-only">Your Company</span>
                    <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600" alt="">
                </a>
                <a href="#" class="text-2xl font-semibold leading-6 pt-1 pl-2 dark:text-white text-gray-900">FTT</a>

            </div>
            <div class="flex lg:hidden">
                <button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700">
                    <span class="sr-only">Open main menu</span>
                    <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                        aria-hidden="true">
                        <path stroke-linecap="round" stroke-linejoin="round"
                            d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                    </svg>
                </button>
            </div>
            <div class="hidden lg:flex lg:gap-x-12">
                <a href="#" class="text-md font-semibold leading-6 dark:text-white text-gray-900">Inicio</a>
                <a href="#" class="text-md font-semibold leading-6 dark:text-white text-gray-900">Proyectos</a>
                <a href="#" class="text-md font-semibold leading-6 dark:text-white text-gray-900">Utilidades</a>
            </div>
            <div class="hidden lg:flex lg:flex-1 lg:justify-end">
                <div class="flex row dark:text-gray-200 text-gray-900 gap-4 justify-start">
                    <div>
                        <a target="_blank" href="https://github.com/felipetrujillot" class="text-2xl">
                            <i class="bi bi-github"></i>
                        </a>
                    </div>

                    <div>
                        <a target="_blank" href="https://www.instagram.com/felipe.itt/" class="text-2xl">
                            <i class="bi bi-instagram"></i>
                        </a>
                    </div>

                    <div>
                        <a href="#" class="text-2xl">
                            <i class="bi bi-twitter"></i>
                        </a>
                    </div>
                    <div @click="updateTheme()" class="border-gray-400 border-l-2 pl-2">
                         <a href="#" class="text-xl"  v-if="theme.darkMode">
                            <i class="bi bi-moon"></i>
                        </a>
                        <a href="#" class="text-2xl" v-else>
                            <i class="bi bi-brightness-high"></i>
                        </a>
                    </div>
                </div>

                <!--  <a href="#" class="text-md font-semibold leading-6 text-white">Log in <span
                        aria-hidden="true">&rarr;</span></a> -->
            </div>
        </nav>
        <!-- Mobile menu, show/hide based on menu open state. -->
        <!-- <div class="lg:hidden" role="dialog" aria-modal="true">
            <div class="fixed inset-0 z-10"></div>
            <div
                class="fixed inset-y-0 right-0 z-10 w-full overflow-y-auto bg-white px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10">
                <div class="flex items-center justify-between">
                    <a href="#" class="-m-1.5 p-1.5">
                        <span class="sr-only">Your Company</span>
                        <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600"
                            alt="">
                    </a>
                    <button type="button" class="-m-2.5 rounded-md p-2.5 text-gray-700">
                        <span class="sr-only">Close menu</span>
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                            aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                        </svg>
                    </button>
                </div>
            </div>
        </div> -->
    </header>
</template>

<script setup lang="ts">
import { reactive } from 'vue'

const theme: { darkMode: boolean } = reactive({
    darkMode: window.matchMedia('(prefers-color-scheme: dark)').matches ?? true
})

const updateTheme = () => {
    theme.darkMode = !theme.darkMode
    theme.darkMode == true ? document.getElementsByTagName('html')[0].classList.add('dark') : document.getElementsByTagName('html')[0].classList.remove('dark')
}
</script>