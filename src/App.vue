<template>
  <router-view />
</template>

<script>
export default {
  created() {
    document.title = 'Sunnyside Agency | Frontend Mentor';
  },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Barlow:wght@600&family=Fraunces:wght@700;900&display=swap');

html,
body {
  margin: 0;
  padding: 0;
}

body {
  font-size: 18px;
  font-family: 'Barlow', sans-serif;
}

h1,
h2,
h3,
button {
  font-family: 'Fraunces', sans-serif;
}
</style>
