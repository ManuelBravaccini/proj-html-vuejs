<script>
export default {
    name: 'CompMatches.vue',

    methods: {
        getIconPath: function (iconPath) {
            return new URL(`../../assets/imgs/${iconPath}.png`, import.meta.url).href
        },
    },
}

</script>

<template>
    <article>
    </article>



</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;
</style>