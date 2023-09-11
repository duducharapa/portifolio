<script setup lang="ts">
import MenuItem from './MenuItem.vue';
import icon from '../assets/coffee.svg';
</script>

<template>
    <header class="header">
        <img :src="icon" class="icon" />

        <ul class="menu">
            <MenuItem link="#about-me">About me</MenuItem>
            <MenuItem link="#projects">Projects</MenuItem>
        </ul>
    </header>
</template>

<style scoped>
    .icon {
        width: 3rem;
    }

    .header {
        width: 100%;
        display: flex;
        align-items: center;
        justify-content: space-between;
        background-color: transparent;
        padding: 30px 64px;
    }

    .menu {
        list-style: none;
        display: flex;
        column-gap: 50px;
    }
</style>