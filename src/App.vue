<template>
  <div id="app">
    <MyHeader />
    <MyContentList />
    <MyFooterTop />
    <MyFooterBottom />

  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyFooterTop from "./components/MyFooterTop.vue";
import MyFooterBottom from "./components/MyFooterBottom.vue";
import MyContentList from "./components/MyContentList.vue";


export default {
  name: "App",
  components: {
    MyHeader,
    MyContentList,
    MyFooterTop,
    MyFooterBottom
  },
};
</script>

<style lang="scss">
@import "./components/style/common.scss";
@import "./components/style/variables.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
