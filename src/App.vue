<template>
  <the-header></the-header>

  <router-view />
</template>

<script>
import TheHeader from "./components/TheHeader.vue";

export default {
  components: {
    TheHeader,
  },
  created() {
    document.title = "Sunnyside Agency | Frontend Mentor";
  },
};
</script>

<style lang="scss">

</style>
