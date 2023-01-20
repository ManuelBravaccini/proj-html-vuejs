<script>
import CompSquadCards from './CompSquadCards.vue';

export default {
    name: 'AppSquads',
    components: {
        CompSquadCards,
    }
}
</script>

<template>
    <section class="app-squads">
        <h5 class="sub-title">Out team players</h5>
        <h1 class="title">Meet our squad players</h1>
        <CompSquadCards />
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

section.app-squads {
    display: flex;
    flex-direction: column;
    background-color: $primary-color;
    text-align: center;
    padding: 5rem 0;

    h1.title {
        color: $text-color;
    }

    h5.sub-title {
        color: $secondary-color;
    }
}
</style>