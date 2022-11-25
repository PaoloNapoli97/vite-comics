<script>
export default {
  name: "AppList",
  data() {
    return {
      shop: [
        {
          name: "DIGITAL COMICS",
          image: "buy-comics-digital-comics.png",
        },
        {
          name: "DC MERCHANDiSE",
          image: "buy-comics-merchandise.png",
        },
        {
          name: "SUBSCRIPTION",
          image: "buy-comics-subscriptions.png",
        },
        {
          name: "COMIC SHOP LOCATOR",
          image: "buy-comics-shop-locator.png",
        },
        {
          name: "DC POWER VISA",
          image: "buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<template>
  <main>
    <div class="container shop-options">
      <div class="option" v-for="content in shop">
        <img :src="`src/assets/img/${content.image}`" alt="{{content.name}}" />
        <p>
          <a href="http://">{{ content.name }}</a>
        </p>
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
main {
  background-color: var(--primary-color);
}
.shop-options {
  padding: 50px 0;
  display: flex;
  justify-content: space-between;

  .option {
    display: flex;
    align-items: center;
    color: var(--secondary-color);

    img {
      width: 40px;
    }

    p {
      padding-left: 10px;

      a {
        text-decoration: none;
        color: inherit;
      }
    }
  }
}
</style>
