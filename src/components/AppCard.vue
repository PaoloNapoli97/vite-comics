<script>
export default {
  name: "AppCard",
  props: {
    img: String,
    series: String,
  },
};
</script>

<template>
  <div class="card">
    <img :src="img" :alt="series" />
    <a href="http://">{{ series }}</a>
  </div>
</template>

<style lang="scss" scoped>
.card {
  margin-top: 14px;
  color: var(--secondary-color);
  a {
    text-decoration: none;
    color: inherit;
  }
}
img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}
</style>
