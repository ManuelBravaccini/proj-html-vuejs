<script>
import CompContacts from './CompsHeader/CompContacts.vue';
import CompNavs from './CompsHeader/CompNavs.vue';

export default {
    name: 'AppHeader',

    components: {
        CompContacts,
        CompNavs,
    },

}

</script>

<template>
    <header>
        <CompContacts />
        <CompNavs />
    </header>
</template>

<style lang="scss">
/*header {
    backdrop-filter: blur(10px);
}*/
</style>