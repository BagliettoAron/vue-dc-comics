<template>
  <div id="app">
    <MyHeader />
    <MyContent />
    <MyFooterTop />
    <MyFooterBottom />

  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyContent from "./components/MyContent.vue";
import MyFooterTop from "./components/MyFooterTop.vue";
import MyFooterBottom from "./components/MyFooterBottom.vue";


export default {
  name: "App",
  components: {
    MyHeader,
    MyContent,
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
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
