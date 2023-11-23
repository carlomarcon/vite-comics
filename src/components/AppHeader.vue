<script>
export default {};
</script>
<template>
  <header>
    <div>
      <div>
        <img src="../assets/img/dc-logo.png" alt="Logo-header" />
      </div>
      <div>
        <ol>
          <li>CHARACTERS</li>
          <li>COMICS</li>
          <li>MOVIES</li>
          <li>TV</li>
          <li>GAMES</li>
          <li>COLLECTIBLES</li>
          <li>VIDEOS</li>
          <li>FANS</li>
          <li>NEWS</li>
          <li>SHOP</li>
        </ol>
      </div>
    </div>
  </header>
</template>
<style lang="scss">
header {
  padding: 2rem;
  height: 40vh;
  width: 100%;

  div {
    height: 100%;
    display: flex;
    justify-content: center;

    div {
      text-align: center;
      padding: 20px;
      img {
        width: 50px;
        height: 50px;
      }
    }

    div {
      li {
        display: inline-block;
        margin: 10px;
      }
    }
  }
}
</style>
