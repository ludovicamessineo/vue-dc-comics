<template>
  <div class="container header__wrapper">
    <div class="header__logo">
      <img src="../assets/dc-logo.png" alt="" />
    </div>
    <div class="header__menu">
      <ul>
        <li
          v-for="(item, index) in listMenu"
          :key="index"
          :class="{ active: item.active }"
        >
          <a href=""> {{ item.text }} </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
  data: function () {
    return {
      listMenu: [
        {
          text: "Character",
          active: false,
        },
        {
          text: "Comics",
          active: true,
        },
        {
          text: "Movies",
          active: false,
        },
        {
          text: "Tv",
          active: false,
        },
        {
          text: "Games",
          active: false,
        },
        {
          text: "Collectibles",
          active: false,
        },
        {
          text: "Videos",
          active: false,
        },
        {
          text: "Fans",
          active: false,
        },
        {
          text: "News",
          active: false,
        },
        {
          text: "Shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.header {
  &__wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  &__logo {
    height: 80px;
  }

  &__logo > img {
    width: 50px;
    margin: 0.5rem;
  }

  &__menu {
    ul {
      display: flex;
    }

    li {
      list-style: none;
      padding: 0.3rem;
      text-transform: uppercase;
      font-size: 0.8rem;
      font-weight: 500;
      color: #303030;

    &.active {
        color: #0282f9;;
    }

        
    }
  }
}
</style>
