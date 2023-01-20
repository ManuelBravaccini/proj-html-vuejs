<script>
import { store } from '../store';

export default {
    name: 'CompVersusCards.vue',
    data() {
        return {
            store,
        }
    },

    methods: {
        getIconPath: function (iconPath) {
            return new URL(`../../assets/imgs/${iconPath}.png`, import.meta.url).href
        },
    },
}

</script>

<template>
    <article>
        <img :src="getIconPath(store.squads[0].logo)" alt="Squad logo">
        <img class="versus-logo" src="../../assets/imgs/vs.png" alt="Versus">
        <img :src="getIconPath(store.squads[1].logo)" alt="Squad logo">
    </article>
    <article>
        <img :src="getIconPath(store.squads[2].logo)" alt="Squad logo">
        <img class="versus-logo" src="../../assets/imgs/vs.png" alt="Versus">
        <img :src="getIconPath(store.squads[3].logo)" alt="Squad logo">
    </article>
    <article>
        <img :src="getIconPath(store.squads[4].logo)" alt="Squad logo">
        <img class="versus-logo" src="../../assets/imgs/vs.png" alt="Versus">
        <img :src="getIconPath(store.squads[5].logo)" alt="Squad logo">
    </article>



</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

article {
    height: 150px;
    display: flex;
    align-items: center;
    background-color: $primary-color-light;
    border-radius: 5px;
    margin: 1rem .5rem 0;

    img {
        height: 75px;
        margin: .5rem;
    }

    img.versus-logo {
        height: 30px;
    }

}
</style>