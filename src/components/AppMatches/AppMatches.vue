<script>
export default {
    name: 'AppMatches',
}
</script>

<template>
    <section>
        <div class="container">
            <h5 class="sub-title">Anywere, anytime</h5>
            <h1 class="title">All matches schedule</h1>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use './styles/partials/variables' as *;

section {
    background-image: url('../../assets/imgs/bg (1).jpg');
    background-size: cover;
    height: 960px;
    display: flex;
    flex-direction: column;

    h1.title {
        color: $text-color;
    }

    h5.sub-title {
        color: $secondary-color;
    }
}
</style>