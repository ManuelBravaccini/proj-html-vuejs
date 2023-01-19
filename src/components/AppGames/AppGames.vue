<script>
import CompVersusCards from './CompVersusCards.vue';

export default {
    name: 'AppGames',

    components: {
        CompVersusCards,
    },
}
</script>

<template>
    <section>
        <div class="container">
            <p>Today's</p>
            <h1>Our game collection</h1>
            <div>
                <CompVersusCards />
            </div>
            <button>Browse all games</button>
            <hr>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

section {
    padding: 5rem 0;
    color: $text-color;
    background-color: $primary-color;
    text-transform: uppercase;

    h1 {
        font-weight: bold;

    }

    p {
        color: $secondary-color;
    }

    .container {
        margin: 0 auto;
        max-width: 960px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    div {
        display: flex;
        justify-content: space-between;
    }

    button {
        margin-top: 2rem;
        padding: 1rem;
        font-weight: bold;
        text-transform: uppercase;
        color: $secondary-color;
        background-color: $text-color;
        border-radius: 5px;
    }

    hr {
        width: 100%;
        margin: 5rem 0;
        border-color: #292a43;
    }
}
</style>