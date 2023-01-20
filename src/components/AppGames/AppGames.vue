<script>
import CompVersusCards from './CompVersusCards.vue';

export default {
    name: 'AppGames',

    components: {
        CompVersusCards,
    },
}
</script>

<template>
    <section>
        <div class="container">
            <h5>Today's</h5>
            <h1>Our game collection</h1>
            <div class="versus-cards">
                <CompVersusCards />
            </div>
            <button>Browse all games</button>
            <hr>
            <div class="pro-team">
                <img src="../../assets/imgs/01.png" alt="Girl gamer">
                <aside>
                    <h5>Who we are</h5>
                    <h1>We are professional team esport</h1>
                    <p>Distinctly provide acces mutfuncto users whereas transparent processes somes ncentivizie
                        eficient functionalities rather than an extensible archtectur services and cross</p>
                    <div class="achievements">
                        <img class="icon-stats" src="../../assets/imgs/icon-1.png" alt="Gamepad">
                        <div>
                            <h3>103K COMMUNITY EARNING</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia tempora quae natus voluptas
                                exercitationem ea praesentium.</p>
                        </div>
                    </div>
                    <div class="achievements">
                        <img class="icon-stats" src="../../assets/imgs/icon-2.png" alt="Gamepad">
                        <div>
                            <h3>34M+ REGISTERED PLAYERS</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia tempora quae natus voluptas
                                exercitationem ea praesentium.</p>
                        </div>
                    </div>
                    <div class="achievements">
                        <img class="icon-stats" src="../../assets/imgs/icon-3.png" alt="Gamepad">
                        <div>
                            <h3>240K STREAMS COMPLETE</h3>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia tempora quae natus voluptas
                                exercitationem ea praesentium.</p>
                        </div>
                    </div>
                </aside>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

section {
    padding: 5rem 0;
    color: $text-color;
    background-color: $primary-color;

    h1,
    h5 {
        margin-bottom: 1rem;
        text-transform: uppercase;
    }

    h1 {
        font-weight: bold;
        font-size: 2rem;
    }

    h5 {
        color: $secondary-color;
    }

    .container {
        margin: 0 auto;
        max-width: 960px;
        display: flex;
        flex-direction: column;
        align-items: center;

        div.versus-cards {
            display: flex;
            justify-content: space-between;
        }

        button {
            margin-top: 2rem;
            padding: 1rem;
            font-weight: bold;
            text-transform: uppercase;
            color: $secondary-color;
            background-color: $text-color;
            border-radius: 5px;
        }

    }

    hr {
        width: 100%;
        margin: 5rem 0;
        border-color: #292a43;
    }

    div.pro-team {
        display: flex;
        align-items: center;
        width: 100%;

        img {
            width: 50%;
        }

        div.achievements {
            display: flex;
            margin: 2rem 0;

            img.icon-stats {
                margin-right: 1rem;
                height: 50px;
                width: 50px;
                padding: .75rem;
                border-radius: 50%;
                background-color: $secondary-color;
            }
        }
    }

}
</style>