<template>
  <div>
    <header class="header">
      <div class="header__logo">
        <img src="../assets/img/dc-logo-bg.png" alt="" />
      </div>
      <div class="header__menu">
        <ul>
          <li
            v-for="(item, index) in navItems"
            :key="index"
            :class="{ active: item.active }"
            >
            <a 
            href=""
            :class="{ activeText: item.active }" 
            >{{ item.text.toUpperCase() }}</a>
          </li>
        </ul>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  name: "MyHeader",
  data: function () {
    return {
      navItems: [
        {
          text: "characters",
          active: false,
        },
        {
          text: "comics",
          active: true,
        },
        {
          text: "movies",
          active: false,
        },
        {
          text: "tv",
          active: false,
        },
        {
          text: "games",
          active: false,
        },
        {
          text: "collectibles",
          active: false,
        },
        {
          text: "videos",
          active: false,
        },
        {
          text: "fans",
          active: false,
        },
        {
          text: "news",
          active: false,
        },
        {
          text: "shop",
          active: false,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "./style/variables.scss";

.header {
  margin-top: 5rem;
  background-color: $nav-background-color;
  display: flex;
  justify-content: space-around;
  line-height: 7rem;

  &__logo {
    display: flex;
    align-items: center;

    img {
      width: 5rem;
    }
  }
}

.header__menu ul {
  display: flex;

  li {
    margin-right: 2rem;
    border-bottom: 4px solid inherit;
    

    a {
      font-weight: 600;
      font-size: 0.8rem;
    }
  }
}

.active {
  border-bottom: 4px solid $selected-and-bluBanner-background-color;
}

.activeText{
    color: $selected-and-bluBanner-background-color; ;
}

</style>
