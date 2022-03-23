<template>
  <div id="app">
    <HeaderDCcomics></HeaderDCcomics>
    <MainDCcomics></MainDCcomics>
    <FooterDCcomics></FooterDCcomics>
  </div>
</template>

<script>
import MainDCcomics from "./components/MainDCcomics.vue";
import HeaderDCcomics from "./components/HeaderDCcomics.vue";
import FooterDCcomics from "./components/FooterDCcomics.vue";

export default {
  name: "App",
  components: {
    HeaderDCcomics,
    MainDCcomics,
    FooterDCcomics,
  },
};
</script>

<style lang="scss">
@import "./assets/styles/partials/_reset.scss";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
}
</style>
