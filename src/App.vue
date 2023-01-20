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


// Button layouts
.btn-white {
  margin: 2rem 0;
  font-weight: bold;
  padding: .8rem 1rem;
  text-transform: uppercase;
  color: $secondary-color;
  background-color: $text-color;
  border-radius: 4px;
  border-width: 0;
  box-shadow: rgba(45, 35, 66, 0.4) 0 2px 4px, rgba(45, 35, 66, 0.3) 0 7px 13px -3px, #D6D6E7 0 -3px 0 inset;
  box-sizing: border-box;
  cursor: pointer;
  transition: box-shadow .15s, transform .15s;
  touch-action: manipulation;
}

.btn-white:focus {
  box-shadow: #D6D6E7 0 0 0 1.5px inset, rgba(45, 35, 66, 0.4) 0 2px 4px, rgba(45, 35, 66, 0.3) 0 7px 13px -3px, #D6D6E7 0 -3px 0 inset;
}

.btn-white:hover {
  box-shadow: rgba(45, 35, 66, 0.4) 0 4px 8px, rgba(45, 35, 66, 0.3) 0 7px 13px -3px, #D6D6E7 0 -3px 0 inset;
  transform: translateY(-2px);
}

.btn-white:active {
  box-shadow: #D6D6E7 0 3px 7px inset;
  transform: translateY(2px);
}

.btn-secondary {
  margin: 2rem 0;
  font-weight: bold;
  padding: .8rem 1rem;
  text-transform: uppercase;
  color: $text-color;
  background-color: $secondary-color;
  border-radius: 4px;
  border-width: 0;
  box-shadow: rgba(45, 35, 66, 0.4) 0 2px 4px, rgba(45, 35, 66, 0.3) 0 7px 13px -3px, #D6D6E7 0 -3px 0 inset;
  box-sizing: border-box;
  cursor: pointer;
  transition: box-shadow .15s, transform .15s;
  touch-action: manipulation;
}

.btn-secondary:focus {
  box-shadow: #D6D6E7 0 0 0 1.5px inset, rgba(45, 35, 66, 0.4) 0 2px 4px, rgba(45, 35, 66, 0.3) 0 7px 13px -3px, #D6D6E7 0 -3px 0 inset;
}

.btn-secondary:hover {
  box-shadow: rgba(45, 35, 66, 0.4) 0 4px 8px, rgba(45, 35, 66, 0.3) 0 7px 13px -3px, #D6D6E7 0 -3px 0 inset;
  transform: translateY(-2px);
}

.btn-secondary:active {
  box-shadow: #D6D6E7 0 3px 7px inset;
  transform: translateY(2px);
}
</style>