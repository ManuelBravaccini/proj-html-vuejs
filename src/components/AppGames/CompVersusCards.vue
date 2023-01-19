<script>
export default {
    name: 'CompVersusCards.vue',
    data() {
        return {
            squads: [
                {
                    name: 'Gaming1',
                    logo: 'team-1',
                },
                {
                    name: 'Gaming2',
                    logo: 'team-2',
                },
                {
                    name: 'Monkey',
                    logo: 'teamsm-4',
                },
                {
                    name: 'Frogs',
                    logo: 'teamsm-3',
                },
                {
                    name: 'Wolves',
                    logo: 'teamsm-2',
                },
                {
                    name: 'Dragons',
                    logo: 'teamsm-1',
                },
            ],
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
        <img :src="getIconPath(squads[0].logo)" alt="Squad logo">
        <img class="versus-logo" src="../../assets/imgs/vs.png" alt="Versus">
        <img :src="getIconPath(squads[1].logo)" alt="Squad logo">
    </article>
    <article>
        <img :src="getIconPath(squads[2].logo)" alt="Squad logo">
        <img class="versus-logo" src="../../assets/imgs/vs.png" alt="Versus">
        <img :src="getIconPath(squads[3].logo)" alt="Squad logo">
    </article>
    <article>
        <img :src="getIconPath(squads[4].logo)" alt="Squad logo">
        <img class="versus-logo" src="../../assets/imgs/vs.png" alt="Versus">
        <img :src="getIconPath(squads[5].logo)" alt="Squad logo">
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