<template>
    <div class="flex">
        <div class="w-64 p-4 bg-base-100 text-base-content">
            <div class="text-2xl font-bold mb-4">Our Services</div>
            <ul class="menu py-3 shadow-lg bg-base-100">
                <li class="menu-title">
                    <span>Delivery</span>
                </li>
                <li class="menu-title">
                    <span>Master classes</span>
                </li>
                <li class="menu-title">
                    <span>Custom cake orders</span>
                </li>
                <li class="menu-title">
                    <span>Consultation</span>
                </li>
            </ul>
        </div>
        <div class="flex gap-10">
            <div class="w-96 p-4 bg-base-100 text-base-content">
                <div class="stats stats-vertical">
                    <div class="stat bg-base-100">
                        <div class="stat-value">Более миллиарда</div>
                        <div class="stat-title">Наименований кондитерских изделий</div>
                    </div>
                    <div class="stat bg-base-100">
                        <div class="stat-value">Дохуйлион</div>
                        <div class="stat-title">Производственных линий</div>
                    </div>
                    <div class="stat bg-base-100">
                        <div class="stat-value">1 мешок</div>
                        <div class="stat-title">Готовой продукции в год</div>
                    </div>
                    <div class="stat bg-base-100">
                        <div class="stat-value">1849 г. до н.э.</div>
                        <div class="stat-title">Год основания фабрики</div>
                    </div>
                </div>
            </div>
            <div class="card w-96 bg-base-100 shadow-xl">
                <figure>
                    <img :src="'museum-tour.webp'" alt="Museum" />
                </figure>
                <div class="card-body">
                    <div class="card-title">Приглашаем на экскурсию по музею</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from "vue";

const services = ref(["Delivery", "Master classes", "Custom cake orders", "Consultation"]);
</script>
