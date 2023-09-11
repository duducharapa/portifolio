<script setup lang="ts">
interface MenuItemProps {
    link: string
}

defineProps<MenuItemProps>();
</script>

<template>
    <li>
        <a class="menu-item-link" :href="link">
            <slot></slot>
        </a>
    </li>
</template>

<style scoped>
    .menu-item-link {
        color: var(--white);
        transition: 0.5s;
        font-size: 1.2rem;
        font-weight: 400;
    }

    .menu-item-link:hover {
        color: #E77637;
    }
</style>