<template>
    <div>
        <nav class="navbar bg-base-100">
            <div class="navbar-start">
                <span>
                    <RouterLink to="/" class="btn btn-ghost text-xl">Красный Октябрь</RouterLink>
                </span>
            </div>
            <div class="navbar-center hidden lg:flex">
                <div class="menu menu-horizontal gap-2">
                    <RouterLink to="/about" class="btn">О нас</RouterLink>
                    <RouterLink to="/products" class="btn">Продукция</RouterLink>
                    <RouterLink to="/store" class="btn">Магазин</RouterLink>
                    <RouterLink to="/contacts" class="btn">Контакты</RouterLink>
                </div>
            </div>
            <div class="navbar-end">
                <div class="menu menu-horizontal gap-2">
                    <RouterLink to="/cart" class="btn">Тележка</RouterLink>
                    <RouterLink to="/login" class="btn">Вход</RouterLink>
                </div>
            </div>
        </nav>
    </div>
    <RouterView />
</template>

<script setup lang="ts"></script>
