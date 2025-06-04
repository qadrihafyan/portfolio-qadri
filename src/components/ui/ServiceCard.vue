<template>
    <div id="Service"
        class="bg-white/10 backdrop-blur p-6 rounded-xl shadow hover:shadow-lg hover:scale-105 transform transition duration-300 text-center"
        data-aos="fade-right">
        <div
            class="w-14 h-14 mx-auto mb-4 flex items-center justify-center rounded-full bg-secondary/20 text-secondary text-2xl">
            <img :src="icon" alt="Service Icon" class="w-8 h-8" />
        </div>
        <h3 class="text-lg font-semibold text-secondary">{{ title }}</h3>
        <p class="text-sm text-white/80 mt-2">{{ description }}</p>
    </div>
</template>

<script setup>
import { defineProps } from 'vue'

defineProps({
    icon: String,
    title: String,
    description: String,
})
</script>
