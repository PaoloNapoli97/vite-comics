<script>
import AppMainNav from "./AppMainNav.vue";
import AppHero from "./AppHero.vue";

export default {
  name: "AppHeader",
  components: {
    AppMainNav,
    AppHero,
  },
};
</script>

<template>
  <header class="container">
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="" />
    </div>
    <AppMainNav />
  </header>
  <AppHero />
</template>

<style lang="scss" scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100px;
}

.logo {
  img {
    width: 70px;
    height: 70px;
  }
}
</style>
