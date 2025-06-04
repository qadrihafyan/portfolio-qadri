<script setup>
defineProps({
    icon: String,
    title: String,
    description: String,
    codeLink: {
        type: String,
        default: 'test',
    },
})
</script>

<template>
    <div
        class="bg-white/20 backdrop-blur p-4 rounded-lg shadow hover:shadow-lg transition text-center flex flex-col justify-between h-full">
        <div>
            <img :src="icon" alt="" class="w-auto h-64 mx-auto mb-3 border-10 rounded-3xl border-primary" />
            <h3 class="text-lg font-semibold text-secondary">{{ title }}</h3>
            <p class="text-sm text-white">{{ description }}</p>
        </div>

        <!-- Tombol View Code -->
        <div v-if="codeLink" class="mt-4">
            <a :href="codeLink" target="_blank" rel="noopener noreferrer"
                class="inline-block mt-auto text-sm px-4 py-2 border bg-secondary text-primary font-semibold rounded-md hover:bg-secondary hover:text-white transition">
                View Code
            </a>
        </div>
    </div>
</template>


