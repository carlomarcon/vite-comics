<script>
export default {
  props: {
    type: Boolean,
    img: String,
    series: String,
    price: String,
  },
  getImagepath(img) {
    return new URL(`../assets/img/${img}`, import.meta.url).href;
  },
};
</script>
<template>
  <div class="card" :class="type">
    <img :src="img" alt="" />
    <h2>
      {{ series }}\ <span>{{ price }}</span>
    </h2>
  </div>
</template>
<style lang="scss" scoped>
.card {
  img {
    height: 200px;
    width: 200px;
  }

  h2 {
    font-size: 18px;
  }

  span {
    font-size: 16px;
  }
}
</style>
