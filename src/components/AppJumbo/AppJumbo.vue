<script>
import AppHeader from './AppHeader/AppHeader.vue';

export default {
    name: 'AppJumbo',

    components: {
        AppHeader,
    },

}

</script>

<template>
    <div class="background">
        <div class="container">
            <section class="jumbo">
                <AppHeader />
                <aside>
                    <h1 id="online-game">Online game</h1>
                    <h2>Genuine money transaction</h2>
                    <p>
                        Assertively Communicate An Expanded Array Of Mindshare Rather Than Diverse Technologies For
                        Magnetic
                        Applications Eamlessly Virtual Then Conveniently Monetize Synergistic Human Capital
                    </p>
                    <button class="btn-white">Join us today</button>
                </aside>
            </section>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

.background {
    background-image: url('../../assets/imgs/bg.jpg');
    background-size: cover;

    .container {
        margin: 0 auto;
        max-width: 960px;

        section.jumbo {
            color: $text-color;

            aside {
                width: 50%;
                padding: 14rem 0;
                line-height: 1.8rem;

                h1,
                h2 {
                    text-transform: uppercase;
                }

                #online-game {
                    font-size: 5rem;
                    margin-bottom: 2rem;
                }
            }
        }
    }


}
</style>