<template>
    <swiper
        :slides-per-view="3"
        :space-between="50"
        @swiper="onSwiper"
        @slideChange="onSlideChange"
        class="flex-shrink"
    >
        <swiper-slide v-for="i in 5" :key="i"> hi {{ i }} </swiper-slide>
    </swiper>
</template>

<script setup lang="ts">
import "swiper/css";
import { Swiper, SwiperSlide } from "swiper/vue";

const onSwiper = (swiper: any) => {
    console.log(swiper);
};
const onSlideChange = () => {
    console.log("slide change");
};
</script>
