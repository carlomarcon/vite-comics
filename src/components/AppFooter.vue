<script>
export default {};
</script>
<template>
  <footer>
    <button>SING-UP NOW!</button>
    <ul>
      <li>FOLLOW US</li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
      <li></li>
    </ul>
  </footer>
</template>
<style lang="scss" scoped>
footer {
  position: relative;
  z-index: 1;
  height: 15%;
  width: 100%;
  background-color: black;
  display: flex;
  justify-content: space-between;
  align-items: center;

  button {
    width: 150px;
    height: 50px;
    background-color: black;
    color: white;
    border: solid 1px cornflowerblue;
  }

  ul {
    list-style-type: none;

    li {
      color: blue;
    }
  }
}
</style>
