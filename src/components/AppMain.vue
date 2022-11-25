<script>
import SectionProducts from "./SectionProducts.vue";
import AppList from "./AppList.vue";

export default {
  name: "AppMain",
  components: {
    SectionProducts,
    AppList,
  },
};
</script>

<template>
  <SectionProducts />
  <AppList />
</template>

<style lang="scss" scoped></style>
