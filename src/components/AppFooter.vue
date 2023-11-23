<script>
export default {
  data() {
    return {
      logoArray: [
        "footer-facebook.png",
        "footer-twitter.png",
        "footer-youtube.png",
        "footer-pinterest.png",
        "footer-periscope.png",
      ],
    };
  },
  methods: {
    getImagepath(img) {
      return new URL(`../assets/img/${img}`, import.meta.url).href;
    },
  },
};
</script>
<template>
  <footer>
    <button>SING-UP NOW!</button>
    <ul>
      <li>FOLLOW US</li>
      <li v-for="(element, index) in logoArray">
        <img :src="getImagepath(logoArray[index])" alt="" />
      </li>
    </ul>
  </footer>
</template>
<style lang="scss" scoped>
footer {
  position: relative;
  z-index: 1;
  height: 15%;
  width: 100%;
  background-color: #303030;
  display: flex;
  justify-content: space-between;
  align-items: center;

  button {
    width: 150px;
    height: 50px;
    background-color: black;
    color: white;
    border: solid 1px #0282f9;
  }

  ul {
    list-style-type: none;

    li {
      color: #0282f9;
      display: inline-block;
      margin: 8px;

      img {
        vertical-align: middle;
        height: 30px;
        width: 30px;
      }
    }
  }
}
</style>
