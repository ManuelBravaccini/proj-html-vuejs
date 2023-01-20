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
        <section class="play-together container">
            <aside>
                <h5 class="sub-title">Let's play together</h5>
                <h1 class="title">Join <span>gamer</span> esports to become next pro gamer today</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam quae distinctio minus id aliquam!
                    Quas
                    animi exercitationem vitae nam, neque sequi eveniet explicabo aliquam praesentium harum accusantium
                    repellendus, optio aliquid!</p>
                <button class="btn-white">Join community</button>
            </aside>
            <div>
                <img src="../../assets/imgs/01 (1).png" alt="Gamers">
            </div>
        </section>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;


p,
h1.title {
    color: $text-color;
}

section.app-squads {
    display: flex;
    flex-direction: column;
    background-color: $primary-color;
    text-align: center;
    padding: 5rem 0;


    h5.sub-title {
        color: $secondary-color;
    }

    section.play-together {
        width: 100%;
        background-image: url('../../assets/imgs/bg\ \(4\).jpg');
        background-size: cover;
        flex-direction: row;

        aside {
            width: 50%;
            text-align: start;
            padding: 2rem;
        }

        span {
            color: $secondary-color;
        }
    }
}
</style>