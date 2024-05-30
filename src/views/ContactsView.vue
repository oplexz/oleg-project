<template>
    <div class="my-10 flex flex-col gap-4 text-center">
        <div class="flex flex-col items-center justify-center gap-8">
            <div class="font-bold text-5xl">Наш адрес</div>
            <div class="flex items-center justify-center gap-10 text-2xl">
                <div class="">107410, г. Москва, ул. Малая Красносельская, 7 стр. 24</div>
                <div class="btn" @click="toggleMap">Схема проезда</div>
                <div class="relative overflow-hidden" v-show="showMap">
                    <div style="position: relative; overflow: hidden">
                        <a
                            href="https://yandex.ru/maps/213/moscow/?utm_medium=mapframe&utm_source=maps"
                            style="color: #eee; font-size: 12px; position: absolute; top: 0px"
                        >
                            Москва
                        </a>
                        <a
                            href="https://yandex.ru/maps/213/moscow/house/malaya_krasnoselskaya_ulitsa_7s24/Z04YcAJnTEYPQFtvfXt5dntqZQ==/?indoorLevel=1&ll=37.657404%2C55.787752&utm_medium=mapframe&utm_source=maps&z=17"
                            style="color: #eee; font-size: 12px; position: absolute; top: 14px"
                        >
                            Малая Красносельская улица, 7с24 на карте Москвы, ближайшее метро Красносельская —
                            Яндекс Карты
                        </a>
                        <iframe
                            src="https://yandex.ru/map-widget/v1/?indoorLevel=1&ll=37.657404%2C55.787752&mode=whatshere&utm_source=share&whatshere%5Bpoint%5D=37.657538%2C55.787791&whatshere%5Bzoom%5D=17&z=17"
                            width="560"
                            height="400"
                            frameborder="1"
                            allowfullscreen="true"
                            style="position: relative"
                        ></iframe>
                    </div>
                </div>
            </div>
            <div class="divider"></div>
            <div class="flex flex-col items-center justify-center gap-8">
                <div class="font-bold text-5xl">Приемная фабрики</div>
                <div class="text-xl">
                    <div class="text-neutral">Телефон приемной</div>
                    <div class=""><a href="tel:+74959825601">+7 (495) 982-56-01</a></div>
                </div>
                <div class="text-xl">
                    <div class="text-neutral">Факс приемной</div>
                    <div class=""><a href="tel:+74959825602">+7 (495) 982-56-02</a></div>
                </div>
            </div>
            <div class="divider"></div>
            <div class="flex flex-col items-center justify-center gap-8">
                <div class="font-bold text-5xl">Канцелярия фабрики</div>
                <div class="text-xl">
                    <div class="text-neutral">Телефон канцелярии</div>
                    <div class=""><a href="tel:+74959825632">+7 (495) 982-56-32</a></div>
                </div>
                <div class="text-xl">
                    <div class="text-neutral">Факс канцелярии</div>
                    <div class=""><a href="tel:+74959825602">+7 (495) 982-56-02</a></div>
                </div>
                <div class="text-xl">
                    <div class="text-neutral">E-mail</div>
                    <div class=""><a href="mailto:ko@redoct.biz">ko@redoct.biz</a></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from "vue";

const showMap = ref(false);

const toggleMap = () => {
    showMap.value = !showMap.value;
};
</script>
