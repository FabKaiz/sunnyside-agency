<template>
  <section class="hero">
    <the-header></the-header>
    <div class="hero-content">
      <h1 id="main-title">WE ARE CREATIVES</h1>
      <svg width="36" height="114" xmlns="http://www.w3.org/2000/svg">
        <g
          stroke="#FFF"
          stroke-width="6"
          fill="none"
          fill-rule="evenodd"
          stroke-linecap="round"
          stroke-linejoin="round"
        >
          <path d="M18 3v100M3 95.484l15 15 15-15" />
        </g>
      </svg>
    </div>
  </section>
</template>

<script>
import TheHeader from './TheHeader.vue';
export default {
  components: {
    TheHeader,
  },
};
</script>

<style lang="scss" scoped>
.hero {
  background-image: url(../assets/images/desktop/image-header.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
}

#main-title {
  font-size: 52px;
  color: #fff;
  font-weight: 900;
  letter-spacing: 0.6rem;
  padding: 0;
  margin: 0;
  margin-bottom: 6rem;
}

.hero-content {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  padding-top: 25vh;
}
</style>
