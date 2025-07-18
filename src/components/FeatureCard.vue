<template>
    <article class="feature-card" role="img" :aria-label="accessibilityLabel">
        <div class="feature-icon" v-html="icon" aria-hidden="true"></div>
        <h3 class="feature-value">{{ value }}</h3>
        <p class="feature-label">{{ label }}</p>
    </article>
</template>

<script setup>
import { computed } from 'vue'

const props = defineProps({
    icon: {
        type: String,
        required: true
    },
    value: {
        type: String,
        required: true
    },
    label: {
        type: String,
        required: true
    }
})

const accessibilityLabel = computed(() => `${props.label}: ${props.value}`)
</script>

<style scoped>
.feature-card {
    @apply flex flex-col items-center justify-center gap-3 text-white text-center;
    transition: transform 0.2s ease-in-out;
}

.feature-card:hover {
    @apply transform scale-105;
}

.feature-icon {
    @apply w-[67px] h-[66px] flex items-center justify-center;
}

.feature-icon :deep(svg) {
    @apply w-full h-full;
}

.feature-value {
    @apply text-3xl font-semibold text-[#FFE48A] mt-2;
}

.feature-label {
    @apply text-xl font-semibold text-white/90 m-0;
}
</style>
