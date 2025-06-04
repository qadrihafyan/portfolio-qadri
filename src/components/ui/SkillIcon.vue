<script setup>
defineProps({
  icon: String, // path ke icon
  label: String,
})
</script>

<template>
  <div class="flex flex-col items-center gap-2 group transition">
    <div
      class="w-16 h-16 rounded-full bg-white/20 backdrop-blur flex items-center justify-center 
             hover:scale-110 transition hover:bg-white/30"
    >
      <img :src="icon" :alt="label" class="w-8 h-8" />
    </div>
    <span class="text-sm text-white font-medium group-hover:text-secondary transition">
      {{ label }}
    </span>
  </div>
</template>
