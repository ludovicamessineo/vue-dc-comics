<template>
  <div id="app">
    <!-- HEADER -->
    <AppHeader />
    <!-- MAIN -->
    <AppMain />
    <!-- FOOTER -->
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
</style>
