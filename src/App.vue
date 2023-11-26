<script>
import AppBody from "./components/AppBody.vue";
import AppFooter from "./components/AppFooter.vue";

import AppHeader from "./components/AppHeader.vue";

export default {
  components: {
    AppBody,
    AppFooter,
    AppHeader,
  },
};
</script>

<template>
  <section id="Wrapper">
    <AppHeader />
    <AppBody />
    <AppFooter />
  </section>
</template>

<style lang="scss">
@use "./style/general.scss";
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#Wrapper {
  height: 1600px;
  width: 100%;
  background-color: aqua;

  div {
    padding-left: 120px;
    padding-right: 120px;

    .card {
      padding: 0;
      width: calc(100% / 6);
      height: 50%;
    }
  }

  footer {
    padding-left: 140px;
    padding-right: 140px;
  }
}
</style>
