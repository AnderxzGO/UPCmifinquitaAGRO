<script setup>
import { RouterLink } from 'vue-router';
defineProps({
    to: {
        type: String
    }
})
</script>
<template>
    <RouterLink :to="{ name: to }" class="rounded bg-emerald-300 hover:bg-emerald-400 transition-colors font-bold py-2 px-10">
        <slot></slot>
    </RouterLink>
</template>

