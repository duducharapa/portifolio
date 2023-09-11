<script setup lang="ts">
import email from '../../assets/email.svg';
import linkedin from '../../assets/linkedin.svg';
import github from '../../assets/github.svg';

interface SocialButtonProps {
    variant: "linkedin" | "github" | "email",
    link: string
}

const props = defineProps<SocialButtonProps>();

const choosenIcon = () => {
    return {
        "linkedin": linkedin,
        "github": github,
        "email": email
    }[props.variant];
}
</script>

<template>
    <a :href="link" target="_blank">
        <div class="container">
            <img class="icon" :src="choosenIcon()" :alt="variant" />
        </div>
    </a>
</template>

<style scoped>
    .container {
        width: 5.5rem;
        height: 5.5rem;
        border-radius: 100%;
        background-color: var(--primary);
        box-shadow: 2px 3px 5px rgb(38, 34, 34);
        transition: 0.5s ease-out;
        cursor: pointer;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .container:hover {
        transform: scale(1.2);
    }

    .icon {
        width: 2.5rem;
        height: 2.5rem;
    }
</style>