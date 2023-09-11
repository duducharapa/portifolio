<script setup lang="ts">
import school from '../../assets/school.svg';

interface GraduationIconProps {
    name: string;
    duration: string;
}

defineProps<GraduationIconProps>();
</script>

<template>
    <div class="graduation-container">
        <div class="icon-container">
            <img :src="school" />
        </div>

        <div class="graduation-description-container">
            <h4>{{ name }}</h4>
            <p>{{ duration }}</p>
        </div>
    </div>
</template>

<style scoped>
    .graduation-container {
        display: flex;
        flex-direction: row;
        width: 100%;
    }
    
    .icon-container {
        background-color: var(--secondary);
        width: 4.5rem;
        height: 4.5rem;
        border-radius: 100%;
        margin-right: 32px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .graduation-description-container {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        justify-content: center;
    }

    img {
        width: 2.5rem;
    }

    h4 {
        color: var(--secondary);
        font-weight: 600;
    }
</style>