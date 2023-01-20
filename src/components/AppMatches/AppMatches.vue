<script>
import { store } from '../store';
import CompLiveMatch from './CompLiveMatch.vue';
import CompUpMatches from './CompUpMatches.vue';
import CompPreMatches from './CompPreMatches.vue';

export default {
    name: 'AppMatches',
    components: {
        CompLiveMatch,
        CompUpMatches,
        CompPreMatches,
    },
    data() {
        return {
            store,
        }
    },
}
</script>

<template>
    <section class="app-matches">
        <div class="container">
            <h5 class="sub-title">Anywere, anytime</h5>
            <h1 class="title">All matches schedule</h1>
            <CompLiveMatch />
            <section class="all-matches">
                <div class="up-matches">
                    <CompUpMatches />
                </div>
                <div class="pre-matches">
                    <CompPreMatches />
                </div>
            </section>
            <button class="btn-white">Browse all matches</button>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

section.app-matches {
    background-image: url('../../assets/imgs/bg (1).jpg');
    background-size: cover;
    display: flex;
    flex-direction: column;
    padding: 3rem 0;

    h1.title {
        color: $text-color;
    }

    h5.sub-title {
        color: $secondary-color;
    }

    section.all-matches {
        display: flex;
    }
}
</style>