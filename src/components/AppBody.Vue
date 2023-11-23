<script>
export default {
  data() {
    return {
      imgObject: [
        {
          image: "../assets/img/buy-comics-digital-comics.png",
          name: "DIGITAL COMICS",
        },
        {
          image: "../assets/img/buy-comics-merchandise.png",
          name: "DC MERCHANDISE",
        },
        {
          image: "../assets/img/buy-comics-subscriptions.png",
          name: "SUBSCRIPTION",
        },
        {
          image: "../assets/img/buy-comics-shop-locator.png",
          name: "COMIC SHOP LOCATOR",
        },
        {
          image: " ../assets/img/buy-dc-power-visa.svg",
          name: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>
<template>
  <body>
    <div class="Contents">Content goes here..</div>
    <div class="Merchandise">
      <ul>
        <li v-for="element in imgObject">
          <h4>{{ element.name }}</h4>
        </li>
      </ul>
    </div>
    <div class="Item">
      <img src="../assets/img/favicon.ico" alt="" />

      <ul>
        <h3>DC COMICS</h3>
        <li>Characters</li>
        <li>Comics</li>
        <li>Movies</li>
        <li>TV</li>
        <li>Games</li>
        <li>Videos</li>
        <li>News</li>
        <h3>SHOP</h3>
        <li>Shop DC</li>
        <li>Shop DC Collections</li>
      </ul>
      <ul>
        <h3>DC</h3>
        <li>terms Of Use</li>
        <li>Privacy</li>
        <li>Ad Choices</li>
        <li>Advertising</li>
        <li>Jobs</li>
        <li>Subscription</li>
        <li>Talent Workshops</li>
        <li>CPSC Certifications</li>
        <li>Ratings</li>
        <li>Shop Help</li>
        <li>Contact Us</li>
      </ul>
      <ul>
        <h3>SITES</h3>
        <li>DC</li>
        <li>MAD Magazine</li>
        <li>DC Kids</li>
        <li>DC Universe</li>
        <li>DC Power Visa</li>
      </ul>
    </div>
  </body>
</template>
<style lang="scss" scoped>
body {
  height: 70%;
  width: 100%;

  .Contents {
    height: 15%;
    background-color: black;
    display: flex;
    align-items: center;

    color: white;
  }
  .Merchandise {
    height: 25%;
    background-color: deepskyblue;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    position: relative;
    z-index: 1;

    ul {
      list-style-type: none;

      li {
        display: inline-block;
        margin: 1rem;
      }
    }
  }

  .Item {
    position: relative;
    img {
      position: absolute;
      right: 20%;
      top: -12%;
      height: 400px;
      z-index: 0;
      transform: rotate(-25deg);
    }

    height: 60%;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: top;
    display: flex;
    padding-top: 1rem;
    gap: 1rem;
    ul {
      display: inline-block;
      list-style-type: none;

      li {
        color: grey;
      }

      h3 {
        color: white;
        margin-bottom: 1rem;
        margin-top: 1rem;
      }
    }
  }
}
</style>
