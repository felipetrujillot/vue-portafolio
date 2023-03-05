<template>
    <Navbar />
    <main>
        <div class="bg-white dark:bg-black">
            <div class="grid md:grid-cols-7 sm:grid-cols-1 py-20 gap-4 h-100 md:mx-20 sm:mx-10">
                <div class="col-span-4 px-6 lg:px-8">
                    <div class="py-32 sm:py-48 lg:py-56">
                        <div class="hidden sm:mb-8 sm:flex sm:justify-start">
                            <div>
                                <p class="text-2xl font-bold dark:text-gray-200 text-gray-600 leading-6 ring-2 p-3 ring-red-500">¡Bienvenido!
                                </p>
                            </div>
                            <!-- <div
                                class="relative rounded-full py-1 px-3 text-sm leading-6 text-gray-100 ring-1 ring-gray-900/10 hover:ring-gray-900/20">
                                Bienvenido a mi portafolio. <a href="#" class="font-semibold text-indigo-600"><span
                                        class="absolute inset-0" aria-hidden="true"></span>Read more <span
                                        aria-hidden="true">&rarr;</span></a>
                            </div> -->
                        </div>
                        <div class="text-start">
                            <h1 class="text-5xl font-bold tracking-tight dark:text-gray-100 text-gray-900 sm:text-7xl">{{ landing.title }}
                                <span class="border-r-4 pr-2 text-red-500">
                                    {{ landing.role }}
                                </span>
                            </h1>
    
                            <p class="mt-6 text-lg leading-8 text-gray-600">
                                Anim aute id magna aliqua ad ad non deserunt sunt.
                                Qui
                                irure qui lorem cupidatat commodo. Elit sunt amet fugiat veniam occaecat fugiat aliqua.
    
                            </p>
                            <div class="mt-10 flex items-center justify-start gap-x-6">
                                <a href="#"
                                    class="rounded-md bg-red-500 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">Get
                                    started</a>
                                <a href="#" class="text-sm font-semibold leading-6 text-gray-900">Learn more <span
                                        aria-hidden="true">→</span></a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="text-white col-span-3 px-6 lg:px-8 justify-start">
                    <div class="max-w-2xl py-32 sm:py-48 lg:py-56">
                        <img
                            src="https://images.pexels.com/photos/14612871/pexels-photo-14612871.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" />
    
                    </div>
                </div>
            </div>
        </div>

        <!-- <div
            class="absolute inset-x-0 top-[calc(100%-13rem)] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[calc(100%-30rem)]">
            <svg class="relative left-[calc(50%+3rem)] h-[21.1875rem] max-w-none -translate-x-1/2 sm:left-[calc(50%+36rem)] sm:h-[42.375rem]"
                viewBox="0 0 1155 678">
                <path fill="url(#ecb5b0c9-546c-4772-8c71-4d3f06d544bc)" fill-opacity=".3"
                    d="M317.219 518.975L203.852 678 0 438.341l317.219 80.634 204.172-286.402c1.307 132.337 45.083 346.658 209.733 145.248C936.936 126.058 882.053-94.234 1031.02 41.331c119.18 108.451 130.68 295.337 121.53 375.223L855 299l21.173 362.054-558.954-142.079z" />
                <defs>
                    <linearGradient id="ecb5b0c9-546c-4772-8c71-4d3f06d544bc" x1="1155.49" x2="-78.208" y1=".177"
                        y2="474.645" gradientUnits="userSpaceOnUse">
                        <stop stop-color="#9089FC" />
                        <stop offset="1" stop-color="#FF80B5" />
                    </linearGradient>
                </defs>
            </svg>
        </div> -->
    </main>


    <div class="bg-gray-900 text-gray-400 flex flex-row justify-between gap-4 py-10 px-20">
        <div class="row">
            <p>Vue
                <svg class="logo" viewBox="0 0 128 128" width="24" height="24" data-v-01fe52ea="">
                    <path fill="#42b883" d="M78.8,10L64,35.4L49.2,10H0l64,110l64-110C128,10,78.8,10,78.8,10z"
                        data-v-01fe52ea=""></path>
                    <path fill="#35495e" d="M78.8,10L64,35.4L49.2,10H25.6L64,76l38.4-66H78.8z" data-v-01fe52ea=""></path>
                </svg>
            </p>
        </div>
        <div class="">Typescript</div>
        <div class="flex flex-row">
            <div>
            </div>
            <div>
                <a href="#" class="flex flex-row">

                    <span class="h-8 pt-1 pr-2">

                        Tailwind
                    </span>

                    <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=white&white=600" alt="">
                </a>
            </div>
        </div>
    </div>
    <!-- <div class="bw-black grid grid-cols-7">
        <div class="text-white col-span-3 border rounded-sm m-10 bg-purple-900 p-10">

            <code class="language-html" data-lang="html">
                    /**
                    * Cambia el texto de manera dinámica
                    * @author FT
                    */
                    const loopChangeText = () => {

                        if (textStatus.completed == true) {
                            landing.role = landing.role.substring(0, landing.role.length - 1)
                            if (landing.role.length > 0) return
                            textStatus.selected = textStatus.selected + 1
                            if (textStatus.selected >= Object.keys(textos).length) textStatus.selected = 0
                            textStatus.completed = false;
                            return
                        }
                        landing.role = textos[textStatus.selected as keyof Numeros].substring(0, landing.role.length + 1)
                        if (landing.role === textos[textStatus.selected as keyof Numeros]) textStatus.completed = true
                        return
                    }
            </code>
        </div>
    </div> -->

    <div class="py-24 sm:py-32 bg-purple-900">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
            <div class="mx-auto max-w-2xl lg:mx-0">
                <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">From the blog</h2>
                <p class="mt-2 text-lg leading-8 text-gray-600">Learn how to grow your business with our expert advice.</p>
            </div>
            <div
                class="mx-auto mt-10 grid max-w-2xl grid-cols-1 gap-y-16 gap-x-8 border-t border-gray-200 pt-10 sm:mt-16 sm:pt-16 lg:mx-0 lg:max-w-none lg:grid-cols-3">
                <article class="flex max-w-xl flex-col items-start justify-between">
                    <div class="flex items-center gap-x-4 text-xs">
                        <time datetime="2020-03-16" class="text-gray-500">Mar 16, 2020</time>
                        <a href="#"
                            class="relative z-10 rounded-full bg-gray-50 py-1.5 px-3 font-medium text-gray-600 hover:bg-gray-100">Marketing</a>
                    </div>
                    <div class="group relative">
                        <h3 class="mt-3 text-lg font-semibold leading-6 text-gray-900 group-hover:text-gray-600">
                            <a href="#">
                                <span class="absolute inset-0"></span>
                                Boost your conversion rate
                            </a>
                        </h3>
                        <p class="mt-5 text-sm leading-6 text-gray-600 line-clamp-3">Illo sint voluptas. Error voluptates
                            culpa eligendi. Hic vel totam vitae illo. Non aliquid explicabo necessitatibus unde. Sed
                            exercitationem placeat consectetur nulla deserunt vel. Iusto corrupti dicta.</p>
                    </div>
                    <div class="relative mt-8 flex items-center gap-x-4">
                        <img src="https://images.unsplash.com/photo-1519244703995-f4e0f30006d5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
                            alt="" class="h-10 w-10 rounded-full bg-gray-50">
                        <div class="text-sm leading-6">
                            <p class="font-semibold text-gray-900">
                                <a href="#">
                                    <span class="absolute inset-0"></span>
                                    Michael Foster
                                </a>
                            </p>
                            <p class="text-gray-600">Co-Founder / CTO</p>
                        </div>
                    </div>
                </article>

                <!-- More posts... -->
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import Navbar from '@/components/Navbar.vue';
import { reactive, onUnmounted } from 'vue';

const textos = ['Full-Stack Web Developer', 'Full-Stack Mobile Developer', 'UI/UX Designer']

const landing: {
    title: string,
    role: string,
} = reactive({
    title: 'Soy Felipe Trujillo ',
    role: 'Full-Stack Web Developer'
})

type Numeros = {
    0: number,
    1: number,
    2: number,
}

const textStatus: {
    completed: boolean,
    selected: number
} = {
    completed: true,
    selected: 0,
}

/**
 * Cambia el texto de manera dinámica
 * @author FT
 */
const loopChangeText = () => {

    if (textStatus.completed == true) {
        landing.role = landing.role.substring(0, landing.role.length - 1)
        if (landing.role.length > 0) return
        textStatus.selected = textStatus.selected + 1
        if (textStatus.selected >= Object.keys(textos).length) textStatus.selected = 0
        textStatus.completed = false;
        return
    }
    landing.role = textos[textStatus.selected as keyof Numeros].substring(0, landing.role.length + 1)
    if (landing.role === textos[textStatus.selected as keyof Numeros]) textStatus.completed = true
    return
}

const intervaloLoop = setInterval(() => {
    loopChangeText()
}, 300 - Math.random() * 100)

onUnmounted(() => clearInterval(intervaloLoop))
</script>