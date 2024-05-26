<template>
    <!-- <div class="bg-pink-500 hover:bg-pink-600 text-white rounded-full p-2 transition-colors duration-200"> -->
    <div class="btn">
        <RouterLink :to="link">{{ text }}</RouterLink>
    </div>
</template>

<script setup lang="ts">
import { defineProps } from "vue";

defineProps({
    text: {
        type: String,
        required: true,
    },
    link: {
        type: String,
        required: true,
    },
});
</script>
