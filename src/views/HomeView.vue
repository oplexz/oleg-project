<template>
    <div class="flex p-8 gap-2">
        <div class="drawer w-64 p-4 bg-base-100 text-base-content flex flex-col justify-between">
            <div>
                <div class="text-2xl font-bold mb-4">Наши услуги</div>
                <ul class="menu py-3 shadow-lg bg-base-100">
                    <li class="menu-title">
                        <span>Доставка</span>
                    </li>
                    <li class="menu-title">
                        <span>Мастер классы</span>
                    </li>
                    <li class="menu-title">
                        <span>Изготовление тортов на заказ</span>
                    </li>
                    <li class="menu-title">
                        <span>Консультация</span>
                    </li>
                </ul>
            </div>
            <div>Адрес: 107410, г. Москва, ул. Малая Красносельская, 7 стр. 24</div>
        </div>
        <div class="">
            <div class="flex gap-10">
                <div class="w-96 p-4 bg-base-100 text-base-content">
                    <div class="stats stats-vertical">
                        <div class="stat bg-base-100">
                            <div class="stat-value">Более 300</div>
                            <div class="stat-title">Наименований кондитерских изделий</div>
                        </div>
                        <div class="stat bg-base-100">
                            <div class="stat-value">70</div>
                            <div class="stat-title">тыс. тонн готовой продукции в год</div>
                        </div>
                        <div class="stat bg-base-100">
                            <div class="stat-value">35</div>
                            <div class="stat-title">Производственных линий</div>
                        </div>
                        <div class="stat bg-base-100">
                            <div class="stat-value">1849</div>
                            <div class="stat-title">Год основания фабрики</div>
                        </div>
                    </div>
                </div>
                <div class="flex gap-4">
                    <div class="card w-96 bg-base-100 shadow-xl">
                        <figure>
                            <img :src="'museum-tour.webp'" alt="Музей" />
                        </figure>
                        <div class="card-body">
                            <div class="card-title">Приглашаем на экскурсию по музею</div>
                        </div>
                    </div>
                    <div class="card w-96 bg-base-100 shadow-xl">
                        <figure>
                            <img :src="'candy-box.webp'" alt="Коробка конфет" />
                        </figure>
                        <div class="card-body">
                            <div class="card-title">Объединенные кондитеры: 20 лет вместе</div>
                        </div>
                    </div>
                    <div class="card w-96 bg-base-100 shadow-xl">
                        <figure>
                            <img :src="'museum-tour.webp'" alt="Museum" />
                        </figure>
                        <div class="card-body">
                            <div class="card-title">Сеть фирменных магазинов Алёнка</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts"></script>
