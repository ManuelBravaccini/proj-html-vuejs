<script>
import { store } from '../store';

export default {
    name: 'CompMatches.vue',
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
        <div class="torunament-infos">
            CALL OF DUTY TOURNAMENT
            <p>
                {{ store.squads[0].date }} | {{ store.squads[0].time }}
            </p>
            <div class="social-logos">
                <img src="../../assets/imgs/social-1.png" alt="Vimeo logo">
                <img src="../../assets/imgs/social-2.png" alt="YouTube logo">
                <img src="../../assets/imgs/social-3.png" alt="Twitch logo">
            </div>
        </div>
        <img :src="getIconPath(store.squads[1].logo)" alt="Squad logo">
    </article>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

article {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: $text-color;
    padding: 1rem;
    text-align: center;

    img {
        margin: 1rem;
    }

    .social-logos {
        display: flex;
        justify-content: space-between;
    }
}
</style>