<script setup lang="ts">
</script>

<template>
    <footer class="container">
        <ul>
            <li>
                <a href="#about-me">About me</a>
            </li>
            <li>
                <a href="#contact-me">Contact me</a>
            </li>
            <li>
                <a href="#projects">Projects</a>
            </li>
            <li>
                <a href="#main-tools">Main tools</a>
            </li>
            <li>
                <a href="/curriculum.pdf" target="_blank">Curriculum</a>
            </li>
        </ul>
        
        <span>Developed by Eduardo Charapa - All Rights reserved</span>
    </footer>
</template>

<style scoped>
    .container {
        width: 100%;
        background-color: #292929;
        padding: 36px 12px 12px 12px;
        display: flex;
        align-items: center;
        flex-direction: column;
    }

    span {
        font-weight: 200;
    }

    ul {
        display: flex;
        flex-direction: row;
        column-gap: 30px;
        list-style: none;
        margin-bottom: 36px;
    }

    a {
        color: var(--white);
    }

</style>