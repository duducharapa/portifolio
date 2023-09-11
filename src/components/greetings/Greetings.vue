<script setup lang="ts">
import SocialButton from './SocialButton.vue';
import image from '../../assets/saito.png';
</script>

<template>
    <div class="main-container">
        <img :src="image" class="main-image" />

        <div class="greetings-container" id="contact-me">
            <div class="titles-container">
                <h1 class="title">Eduardo Charapa</h1>
                <h2 class="subtitle">Fullstack developer focused on Java and Javascript</h2>
            </div>
            <div>
                <h4>Contact me</h4>

                <div class="social-container">
                    <SocialButton variant="linkedin" link="https://www.linkedin.com/in/eduardo-charapa-48a709199" />
                    <SocialButton variant="github" link="https://github.com/duducharapa" />
                    <SocialButton variant="email" link="mailto:charapadev@gmail.com" />
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .main-image {
        height: 600px;
    }

    .title {
        font-size: 3rem;
        font-weight: 500;
    }

    .subtitle {
        font-weight: 400;
        color: var(--primary);
        font-size: 2rem;
    }

    h4 {
        font-size: 1.5rem;
        text-align: center;
        font-weight: 400;
        margin-bottom: 20px;
    }

    .main-container {
        width: 100%;
        display: flex;
        flex-direction: row;
        justify-content: center;
        padding: 64px 0;
    }

    .greetings-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .titles-container {
        margin-bottom: 50px;
    }

    .social-container {
        display: flex;
        justify-content: center;
        column-gap: 40px;
        width: 100%;
    }
</style>