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
  <section id="Header-section"></section>
  <section id="Body-section"></section>
  <section id="Footer-section"></section>
</template>

<style scoped lang="scss">
@use "./style/general.scss";
</style>
