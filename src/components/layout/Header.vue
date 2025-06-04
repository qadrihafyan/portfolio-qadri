<script setup>
import { ref } from 'vue';
const navItems = ref([
    { name: "Home", href: "#Home" },
    { name: "Skill", href: "#Skill" },
    { name: "Service", href: "#Service" },
    { name: "Project", href: "#Project" },
    { name: "Contact", href: "#Contact" },
])

const isOpen = ref(false)
</script>

<template>
    <div class="sticky top-0 z-20 backdrop-blur-2xl bg-white/20">
        <div class="flex justify-between items-center mx-auto w-full h-16 px-5">
            <div>
                <h1 class="text-secondary text-xl font-bold md:text-3xl">Portfolio</h1>
            </div>
            <nav class="hidden md:block">
                <ul class="flex gap-6">
                    <li v-for="item in navItems" :key="item.name">
                        <a :href="item.href" class="fonst-meduum text-white hover:text-secondary">{{ item.name }}</a>
                    </li>
                </ul>
            </nav>
            <button @click="isOpen = !isOpen" class="focus:outline-none text-white md:hidden">
                <svg v-if="!isOpen" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                </svg>

                <svg v-else class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                </svg>

            </button>
        </div>

        <!-- Menu Mobile -->
        <div v-if="isOpen" class="md:hidden text-white shadow-lg py-5 border-t-1">
            <nav>
                <ul class="flex flex-col gap-2 px-2">
                    <li v-for="item in navItems" :key="item.name" @click="isOpen = false">
                        <a :href="item.href">{{ item.name }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>