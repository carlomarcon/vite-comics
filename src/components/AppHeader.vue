<script>
export default {};
</script>
<template>
  <header>
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="LOGO" />
    </div>
    <div class="list">
      <ul>
        <li>CHARACTERS</li>
        <li>COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTABLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
      </ul>
    </div>
  </header>
</template>
<style lang="scss" scoped>
header {
  width: 100%;
  height: 15%;
  background-color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;

  .logo {
    img {
      width: 80px;
      height: 80px;
    }
  }

  .list {
    ul {
      list-style-type: none;

      li {
        display: inline-block;
        margin: 1rem;
        font-size: 10px;
      }
    }
  }
}
</style>
