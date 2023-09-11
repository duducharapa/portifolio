<script setup lang="ts">
import java from '../../assets/java.svg';
import quarkus from '../../assets/quarkus.png';
import spring from '../../assets/spring.png';
import typescript from '../../assets/typescript.png';
import vue from '../../assets/vue.png';
import react from '../../assets/react.png';

interface StackIconProps {
    variant: "java" | "quarkus" | "spring-boot" | "typescript" | "react" | "vue"
}

interface StackIconData {
    title: string
    image: any
}

const props = defineProps<StackIconProps>();

const resolveVariant = (): StackIconData => {
    return {
        "java": {
            title: "Java",
            image: java
        },
        "quarkus": {
            title: "Quarkus",
            image: quarkus
        },
        "spring-boot": {
            title: "Spring Boot",
            image: spring
        },
        "typescript": {
            title: "Typescript",
            image: typescript
        },
        "react": {
            title: "React",
            image: react
        },
        "vue": {
            title: "Vue",
            image: vue
        }
    }[props.variant];
}

const { title, image } = resolveVariant();
</script>

<template>
    <div class="stack-container">
        <div class="icon-container">
            <img :src="image" class="stack-image" />
        </div>

        <h4>{{ title }}</h4>
    </div>
</template>

<style scoped>
    .stack-container {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .icon-container {
        background-color: var(--white);
        width: 6rem;
        height: 6rem;
        border-radius: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
        margin-bottom: 10px;
    }

    .stack-image {
        width: 3rem;
    }

    h4 {
        font-weight: 400;
        font-size: 1.2rem;
    }
</style>