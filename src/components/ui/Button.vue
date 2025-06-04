<!-- src/components/BaseButton.vue -->
<template>
    <button :class="[
        'px-6 py-3 font-medium rounded-lg transition duration-200',
        variant === 'primary'
            ? 'bg-primary text-white hover:brightness-110'
            : variant === 'secondary'
                ? 'border border-secondary text-secondary hover:bg-secondary hover:text-white'
                : '',
    ]">
        {{ label }}
    </button>
</template>

<script setup>
defineProps({
    variant: {
        type: String,
        default: 'primary'
    },
    label: {
        type: String,
        required: true,
    },
});
</script>
