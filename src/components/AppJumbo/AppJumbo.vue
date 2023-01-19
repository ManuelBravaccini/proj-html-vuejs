<script>
import AppHeader from './AppHeader/AppHeader.vue';

export default {
    name: 'AppJumbo',

    components: {
        AppHeader,
    },

}

</script>

<template>
    <div class="back">

        <div class="container">
            <section class="jumbo">
                <AppHeader />
                <h1>Jumbo</h1>
            </section>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

.background {
    background-image: url('../../assets/imgs/bg.jpg');
    background-size: cover;

    .container {
        margin: 0 auto;
        max-width: 960px;
    }

    section.jumbo {
        height: 100vh;
        color: $text-color;
    }

}
</style>