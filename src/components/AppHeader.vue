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
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
header {
  padding: 2rem;
  height: 15vh;
  width: 100%;
  background-color: white;

  div {
    height: 100%;
    display: flex;
    justify-content: center;

    div {
      text-align: center;
      padding: 20px;
      align-items: center;
      img {
        width: 50px;
        height: 50px;
      }
    }

    div {
      align-items: center;
      li {
        display: inline-block;
        margin: 10px;
      }
    }
  }
}
</style>
