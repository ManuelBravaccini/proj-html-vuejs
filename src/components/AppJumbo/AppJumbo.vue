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
    <AppHeader />
    <section>
        <h1>Jumbo</h1>
    </section>
</template>

<style lang="scss">
section {
    display: flex;
    justify-content: center;
}
</style>