<script>
import { store } from '../store';

export default {
    name: 'CompLiveMatch.vue',
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
    <section class="match-card">
        <div class="prize-pool">
            <h3>2 GROUP 32 PLAYERS</h3>
            <h3>PRIZE POOL $3200</h3>
        </div>
        <article>
            <div>
                <h2>BATTLEFIELD-4 TORNAMENT</h2>
                <p>
                    {{ store.squads[0].date }} | {{ store.squads[0].time }}
                </p>
            </div>
            <img class="squad-logo" :src="getIconPath(store.squads[0].logo)" alt="Squad logo">
            <img class="versus-logo" src="../../assets/imgs/vs.png" alt="Versus">
            <img class="squad-logo" :src="getIconPath(store.squads[1].logo)" alt="Squad logo">
            <div class="social-logos">
                <img src="../../assets/imgs/social-1.png" alt="Vimeo logo">
                <img src="../../assets/imgs/social-2.png" alt="YouTube logo">
                <img src="../../assets/imgs/social-3.png" alt="Twitch logo">
            </div>
        </article>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

section.match-card {
    margin: 2rem;
    width: 100%;
}

div.prize-pool {
    background-color: $secondary-color;
    display: flex;
    justify-content: space-between;
    padding: .5rem;
    color: $text-color;
}

article {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: $text-color;
    padding: 1rem;
    text-align: center;


    img.squad-logo {
        margin: 1rem;
        width: 70px;
    }

    .social-logos {
        display: flex;
        justify-content: center;

        img {
            width: 30px;
            margin: .5rem;
        }
    }
}
</style>