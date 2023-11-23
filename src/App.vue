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
  height: 100vh;
  width: 100%;
  background-color: aqua;

  div {
    padding-left: 120px;
    padding-right: 120px;
  }

  footer {
    padding-left: 120px;
    padding-right: 120px;
  }
}
</style>
