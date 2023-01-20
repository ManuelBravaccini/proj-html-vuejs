<script>
import { store } from '../store';

export default {
    name: 'CompPreMatches.vue',
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
    <h1>PREVIOUS MATCHES</h1>
    <section class="match-card" v-for="(squadEl, index) in store.squads.slice(0, 3)" :key="index">
        <div class="prize-pool">
            <h3>2 GROUP 32 PLAYERS</h3>
            <h3>PRIZE POOL $3200</h3>
        </div>
        <article>
            <img class="squad-logo" :src="getIconPath(squadEl.logo)" alt="Squad logo">
            <div class="torunament-infos">
                <h3>CALL OF DUTY TOURNAMENT</h3>
                <p>
                    {{ store.squads[0].date }} | {{ store.squads[0].time }}
                </p>
                <div class="social-logos">
                    <img src="../../assets/imgs/social-1.png" alt="Vimeo logo">
                    <img src="../../assets/imgs/social-2.png" alt="YouTube logo">
                    <img src="../../assets/imgs/social-3.png" alt="Twitch logo">
                </div>
            </div>
            <img class="squad-logo" :src="getIconPath(squadEl.logo)" alt="Squad logo">
        </article>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

h1 {
    color: $text-color;
    text-align: center;
    margin-bottom: 1rem;
}

section.match-card {
    margin-bottom: 1rem;
    height: 175px;
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
        height: 70px;
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