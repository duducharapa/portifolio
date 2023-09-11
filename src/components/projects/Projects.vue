<script setup lang="ts">
</script>

<template>
    <div class="container" id="projects">
        <h2>Projects</h2>

        <article>
            <h3>Replaydown! API</h3>

            <section>
                <iframe
                    width="560"
                    height="315"
                    src="https://www.youtube.com/embed/mSdU-AS4ZsM?si=rlKPzB7OSD3r3hUx"
                    title="YouTube video player"
                    frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                    allowfullscreen>
                </iframe>

                <div>
                    <p>
                        The Replaydown! API is an application that analyzes the text logs from matches on Pokémon Showdown! game.
                    </p>
                    <p>
                        It is made in 
                        <strong class="mark-primary">Java 17</strong> + 
                        <strong class="mark-primary">Quarkus framework</strong>, also using the reactive programming.
                    </p>

                    <h4>How it works?</h4>
                    <p class="last-paragraph">
                        Every match replay has an ID that can be used to get the text logs. Using this, 
                        <strong class="mark-primary">the application interpretes these lines and transforms it</strong>.
                    </p>

                    <a href="https://github.com/duducharapa/replaydown-api" target="_blank" class="primary-button">Source code</a>
                </div>
            </section>
        </article>

        <article>
            <h3>Premier Brasil</h3>

            <section class="inverse-section">
                <iframe
                    width="560"
                    height="315"
                    src="https://www.youtube.com/embed/mSdU-AS4ZsM?si=rlKPzB7OSD3r3hUx"
                    title="YouTube video player"
                    frameborder="0"
                    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                    allowfullscreen>
                </iframe>

                <div>
                    <p>
                        The Premier Brasil is a project focused on 
                        <strong class="mark-secondary">perform games</strong> 
                        where the 
                        <strong class="mark-secondary">user can win real prizes</strong>.
                    </p>

                    <h4>How I participate?</h4>
                    <p>
                        As a backend developer, I was responsible to 
                        <strong class="mark-secondary">modelling data</strong> 
                        and 
                        <strong class="mark-secondary">build the server side application</strong>.
                    </p>
                    <p class="last-paragraph">
                        The application was built using 
                        <strong class="mark-secondary">Java 17</strong> + <strong class="mark-secondary">Spring Boot</strong>. 
                        For data persistence, the database chosen was 
                        <strong class="mark-secondary">MariaDB</strong> and some tools for deploy like 
                        <strong class="mark-secondary">Jenkins</strong> and <strong class="mark-secondary">Docker</strong> are also used.
                    </p>

                    <a href="https://premierbrasil1bi.com.br" target="_blank" class="secondary-button">Visit site</a>
                </div>
            </section>
        </article>
    </div>
</template>

<style scoped>
    .container {
        width: 100%;
        padding: 64px 64px;
        display: flex;
        flex-direction: column;
        row-gap: 64px;
    }

    h2 {
        font-size: 3rem;
    }

    h3 {
        font-size: 2rem;
    }

    h4 {
        font-size: 1.5rem;
    }

    h3 {
        font-weight: 500;
    }

    p, h3 {
        margin-bottom: 10px;
    }

    strong {
        font-weight: 500;
    }

    .mark-primary {
        color: var(--primary);
    }

    .mark-secondary {
        color: var(--secondary);
    }

    a {
        border-radius: 10px;
        padding: 15px 30px;
        color: var(--white);
        transition: 0.5s;
        font-weight: 700;
    }

    .primary-button {
        background-color: var(--primary);        
    }

    .primary-button:hover {
        background-color: var(--primary-hover);
    }

    .secondary-button {
        background-color: var(--secondary);
    }

    .secondary-button:hover {
        background-color: var(--secondary-hover);
    }

    section {
        display: flex;
        flex-direction: row;
        column-gap: 30px;
    }

    .inverse-section {
        flex-direction: row-reverse;
    }

    .last-paragraph {
        margin-bottom: 30px;
    }
</style>