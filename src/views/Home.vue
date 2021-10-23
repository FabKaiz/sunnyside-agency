<template>
  <div class="home">
    <the-hero></the-hero>
    <services></services>
    <testimonials></testimonials>
    <gallery></gallery>
    <the-footer></the-footer>
  </div>
</template>

<script>
import TheHero from '../components/TheHero.vue';
import Services from '../components/Services.vue';
import Testimonials from '../components/Testimonials.vue';
import Gallery from '../components/Gallery.vue';
import TheFooter from '../components/TheFooter.vue';

export default {
  components: {
    TheHero,
    Services,
    Testimonials,
    Gallery,
    TheFooter,
  },
};
</script>
