<script>
import { store } from '../store';

export default {
    name: 'CompContentLives',
    data() {
        return {
            store,
        }
    },
    methods: {
        getIconPath: function (iconPath) {
            return new URL(`../../assets/imgs/${iconPath}.jpg`, import.meta.url).href
        },
    },
}
</script>

<template>
    <div>
        <article class="live-streamings" v-for="(liveEl, index) in store.lives" :key="index">
            <img :src="getIconPath(liveEl.image)" alt="Lives">
            <button class="btn-secondary">Watch now</button>
            <h1>
                {{ liveEl.title }}
            </h1>
        </article>
    </div>
    <div>
        <article class="videos" v-for="(videoEl, index) in store.videos" :key="index">
            <img :src="getIconPath(videoEl.image)" alt="Videos">
        </article>
    </div>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;


div {
    display: flex;
    justify-content: space-between;
    gap: 10px;
}

article {
    button {
        position: absolute;
        bottom: 2rem;
        left: 2rem;
    }

    h1 {
        position: absolute;
        bottom: 2rem;
        left: 2rem;
        text-transform: uppercase;
        color: $text-color;
    }
}

article.live-streamings {
    margin-bottom: 1rem;
    position: relative;

    img {
        width: 450px;
        border: 10px solid $primary-color-light;
    }
}

article.videos {
    gap: 10px;
    width: 300px;
    height: 300px;

    img {
        width: 300px;
        height: 300px;
        border: 10px solid $primary-color-light;
    }
}
</style>