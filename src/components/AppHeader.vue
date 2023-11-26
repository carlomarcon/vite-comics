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
  height: 8%;
  background-color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;

  .logo {
    display: flex;
    align-items: center;
    img {
      width: 80px;
      height: 80px;
    }
  }

  .list {
    height: 100%;
    display: flex;
    align-items: center;
    padding: 16px;
    padding-top: 41px;
    ul {
      list-style-type: none;
      height: 100%;

      li {
        display: inline-block;
        margin: 1rem;
        font-size: 10px;
        height: 100%;

        &:hover {
          border-bottom: 3px solid blue;
        }
      }
    }
  }
}
</style>
