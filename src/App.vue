<script>
import AppJumbo from './components/AppJumbo/AppJumbo.vue';
import AppGames from './components/AppGames/AppGames.vue';
import AppMatches from './components/AppMatches/AppMatches.vue';
import AppSquads from './components/AppSquads/AppSquads.vue';
import AppLives from './components/AppLives/AppLives.vue';
import AppProducts from './components/AppProducts/AppProducts.vue';
import AppBlogs from './components/AppBlogs/AppBlogs.vue';
import AppTestimonials from './components/AppTestimonials/AppTestimonials.vue';
import AppFooter from './components/AppFooter/AppFooter.vue';

export default {
  name: 'AppVue',

  components: {
    AppJumbo,
    AppGames,
    AppMatches,
    AppSquads,
    AppLives,
    AppProducts,
    AppBlogs,
    AppTestimonials,
    AppFooter,
  },
}
</script>

<template>
  <div class="wrapper">
    <AppJumbo />
    <AppGames />
    <AppMatches />
    <AppSquads />
    <AppLives />
    <AppProducts />
    <AppBlogs />
    <AppTestimonials />
    <AppFooter />
  </div>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables' as *;
</style>
