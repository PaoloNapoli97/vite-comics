<script>
export default {
  name: "AppList",
  data() {
    return {
      shop: [
        {
          name: "Digital Comics",
          image: "buy-comics-digital-comics.png",
        },
        {
          name: "Digital Comics",
          image: "buy-comics-digital-comics.png",
        },
        {
          name: "Digital Comics",
          image: "buy-comics-digital-comics.png",
        },
        {
          name: "Digital Comics",
          image: "buy-comics-digital-comics.png",
        },
      ],
    };
  },
};
</script>

<template>
  <img :src="`../asset/img/${shop.image}`" alt="{{shop.name}}" />
</template>

<style scoped></style>
