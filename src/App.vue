<template>
  <div id="app">
    <MyHeader />
    <MyContent />
    <MyFooterTop />

  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyContent from "./components/MyContent.vue";
import MyFooterTop from "./components/MyFooterTop.vue";


export default {
  name: "App",
  components: {
    MyHeader,
    MyContent,
    MyFooterTop,
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
