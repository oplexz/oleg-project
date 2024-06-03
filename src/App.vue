<template>
    <div class="drawer">
        <input id="my-drawer-3" type="checkbox" class="drawer-toggle" />
        <div class="drawer-content flex flex-col">
            <div class="w-full navbar bg-base-300">
                <div class="flex-none lg:hidden">
                    <label for="my-drawer-3" aria-label="open sidebar" class="btn btn-square btn-ghost">
                        <svg
                            xmlns="http://www.w3.org/2000/svg"
                            fill="none"
                            viewBox="0 0 24 24"
                            class="inline-block w-6 h-6 stroke-current"
                        >
                            <path
                                stroke-linecap="round"
                                stroke-linejoin="round"
                                stroke-width="2"
                                d="M4 6h16M4 12h16M4 18h16"
                            ></path>
                        </svg>
                    </label>
                </div>
                <div class="flex justify-between w-full">
                    <RouterLink to="/" class="btn btn-ghost text-xl">
                        <img :src="'krasniy-oktyabr.svg'" alt="Красный Октябрь" class="h-12" />
                    </RouterLink>
                    <div class="hidden lg:block">
                        <div class="menu menu-horizontal gap-2">
                            <RouterLink to="/about" class="btn">О нас</RouterLink>
                            <RouterLink to="/products" class="btn">Продукция</RouterLink>
                            <RouterLink to="/store" class="btn">Магазин</RouterLink>
                            <RouterLink to="/contacts" class="btn">Контакты</RouterLink>
                        </div>
                    </div>
                    <div class="menu menu-horizontal gap-2">
                        <RouterLink to="/cart" class="btn">Тележка</RouterLink>
                        <RouterLink to="/login" class="btn">Вход</RouterLink>
                    </div>
                </div>
            </div>
            <RouterView />
        </div>
        <div class="drawer-side">
            <label for="my-drawer-3" aria-label="close sidebar" class="drawer-overlay"></label>
            <ul class="menu p-4 w-80 min-h-full bg-base-200">
                <li><RouterLink to="/about">О нас</RouterLink></li>
                <li><RouterLink to="/products">Продукция</RouterLink></li>
                <li><RouterLink to="/store">Магазин</RouterLink></li>
                <li><RouterLink to="/contacts">Контакты</RouterLink></li>
            </ul>
        </div>
    </div>
</template>

<script setup lang="ts"></script>
