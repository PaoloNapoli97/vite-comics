<script>
export default {
  name: "AppMainNav",
  data() {
    return {
      links: [
        {
          href: "#",
          name: "Characters",
          active: false,
        },
        {
          href: "#",
          name: "Comics",
          active: false,
        },
        {
          href: "#",
          name: "Movies",
          active: false,
        },
        {
          href: "#",
          name: "Tv",
          active: false,
        },
        {
          href: "#",
          name: "Games",
          active: false,
        },
        {
          href: "#",
          name: "Collectibles",
          active: false,
        },
        {
          href: "#",
          name: "Videos",
          active: false,
        },
        {
          href: "#",
          name: "Fans",
          active: false,
        },
        {
          href: "#",
          name: "News",
          active: false,
        },
        {
          href: "#",
          name: "Shop",
          active: false,
        },
      ],
    };
  },
  methods: {
    changeLink(index) {
      this.links.forEach((elm, i) => {
        if (i === index) {
          elm.active = true;
        } else {
          elm.active = false;
        }
      });
    },
  },
};
</script>

<template>
  <nav class="main-nav">
    <ul>
      <li v-for="(item, index) in links">
        <a
          :class="{ active: item.active }"
          :href="item.href"
          @click.prevent="changeLink(index)"
          >{{ item.name }}
        </a>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss" scoped>
.main-nav {
  display: flex;

  ul {
    display: flex;
    list-style: none;

    li {
      padding: 10px 20px;
      margin: 0 2px;

      a {
        text-decoration: none;
        color: inherit;

        &.active {
          color: var(--primary-color);
          border-bottom: 4px solid var(--primary-color);
          padding-bottom: 35px;
        }
      }
    }
  }
}
</style>
