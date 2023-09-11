<script setup lang="ts">
import GraduationIcon from './GraduationIcon.vue';
import StackIcon from './StackIcon.vue';
</script>

<template>
    <div class="container" id="about-me">
        <div class="aboutme-container">
            <h2>About me</h2>

            <p>
                Hello! My name is Eduardo Charapa and I am a 
                <strong>fullstack developer</strong>, 
                focused on backend development using <strong>Java</strong>.
            </p>

            <p>
                Even I being focused on this, I know a lot of things like 
                <strong>Devops</strong>, 
                <strong>Networks</strong> and 
                <strong>Cloud computing</strong>.
            </p>

            <h3>Graduations</h3>

            <div class="graduations-list">
                <GraduationIcon id="first-graduation" name="Computer Networks" duration="2017 to 2019" />
                <GraduationIcon name="System Analysis and Development" duration="Finishes on 2023" />
            </div>
        </div>
        <div class="tools-container" id="main-tools">
            <h2>Main tools</h2>

            <div class="tools-list tools-list-first">
                <StackIcon variant="java" />
                <StackIcon variant="quarkus" />
                <StackIcon variant="spring-boot" />
            </div>
            <div class="tools-list">
                <StackIcon variant="typescript" />
                <StackIcon variant="react" />
                <StackIcon variant="vue" />
            </div>
        </div>
    </div>
</template>

<style scoped>
    .container {
        width: 100%;
        background-color: #292929;
        padding: 64px 64px;
        display: flex;
        flex-direction: row;
    }

    .aboutme-container {
        width: 50%;
        padding-right: 40px;
    }

    .tools-container {
        width: 50%;
    }

    .tools-list {
        width: 100%;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .tools-list-first {
        margin-bottom: 30px;
    }

    h2 {
        font-size: 3rem;
    }

    h3 {
        font-size: 2rem;
    }

    h2, h3 {
        margin-bottom: 30px;
        font-weight: 500;
    }

    p, #first-graduation {
        margin-bottom: 20px;
    }

    strong {
        color: var(--primary);
        font-weight: 500;
    }
</style>