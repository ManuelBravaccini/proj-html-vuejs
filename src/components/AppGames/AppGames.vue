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
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

section {
    padding: 5rem 0;
    color: $text-color;
    background-color: $primary-color;

    .container {
        margin: 0 auto;
        max-width: 960px;
        display: flex;
        flex-direction: column;
    }

    div {
        display: flex;
        justify-content: space-between;
    }
}
</style>