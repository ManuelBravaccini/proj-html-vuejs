<script>
import { store } from '../store';

export default {
    name: 'AppSquads',
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
    <section class="squad-card">
        <article v-for="(squadEl, index) in store.squads.slice(0, 5)" :key="index">
            <img class="squad-logo" :src="getIconPath(squadEl.logo)" alt="Squad logo">
            <h5>
                {{ squadEl.name + ' team' }}
            </h5>
            <div class="social-logos">
                <img class="social-logo" src="../../assets/imgs/social-1.png" alt="Vimeo logo">
                <img class="social-logo" src="../../assets/imgs/social-2.png" alt="YouTube logo">
                <img class="social-logo" src="../../assets/imgs/social-3.png" alt="Twitch logo">
            </div>
        </article>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

section.squad-card {
    display: flex;
    overflow: auto;
    gap: 20px;

    article {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 20px;
        width: 350px;
        height: 550px;
        background-image: url('../../assets/imgs/5.jpg');
        background-size: cover;
        border: 10px solid $primary-color-light;

        h5 {
            font-size: 1.5rem;
            text-transform: uppercase;
            color: $text-color;
        }

        img.squad-logo {
            width: 40%;
        }

        img.social-logo {
            width: 50px;
            margin: .5rem;
        }
    }
}


/*
section {
    flex-direction: column;
    background-color: $primary-color;
    height: 960px;
    text-align: center;
    padding: 5rem 0;

    h1.title {
        color: $text-color;
    }

    h5.sub-title {
        color: $secondary-color;
    }
}*/
</style>