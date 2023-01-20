<script>
import CompContentLives from './CompContentLives.vue';

export default {
    name: 'AppLives',
    components: {
        CompContentLives,
    },
}
</script>

<template>
    <section class="lives">
        <div class="container">
            <h5 class="sub-title">Our latest videos</h5>
            <h1 class="title">Check our live streaming</h1>
            <section>
                <CompContentLives />
            </section>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

section.lives {
    background-image: url('../../assets/imgs/bg\ \(3\).jpg');
    padding: 5rem 0;

    div.container {
        flex-wrap: wrap;
    }

    h5 {
        color: $secondary-color;
    }

    h1 {
        color: $text-color;
    }
}
</style>