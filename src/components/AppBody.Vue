<script>
import AppFumets from "./AppFumets.vue";

export default {
  components: {
    AppFumets,
  },
  data() {
    return {
      imgObject: [
        {
          image: "buy-comics-digital-comics.png",
          name: "DIGITAL COMICS",
        },
        {
          image: "buy-comics-merchandise.png",
          name: "DC MERCHANDISE",
        },
        {
          image: "buy-comics-subscriptions.png",
          name: "SUBSCRIPTION",
        },
        {
          image: "buy-comics-shop-locator.png",
          name: "COMIC SHOP LOCATOR",
        },
        {
          image: " buy-dc-power-visa.svg",
          name: "DC POWER VISA",
        },
      ],

      imgFumets: [
        {
          thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg/revision/latest?cb=20080809201655",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg/revision/latest/scale-to-width-down/1200?cb=20130627211607",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg/revision/latest?cb=20200929145132",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg/revision/latest?cb=20200929124651",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg/revision/latest?cb=20201123054610",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://m.media-amazon.com/images/I/91uTUXN0sNS._AC_UF1000,1000_QL80_.jpg",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg/revision/latest?cb=20160303223223",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
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
  <body>
    <div class="Contents">
      <div class="Fumets">
        <AppFumets
          v-for="element in imgFumets"
          :img="element.thumb"
          :price="element.price"
          :series="element.series"
        />
        <!-- <div class="card" :class="type">
    <img :src="img" alt="" />
    <h2>
      {{ series }}\ <span>{{ price }}</span>
    </h2>
  </div> -->
      </div>
    </div>
    <div class="Merchandise">
      <ul>
        <li v-for="element in imgObject">
          <img :src="getImagepath(element.image)" alt="" />
          <span>{{ element.name }}</span>
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
  height: 77%;
  width: 100%;

  .Fumets {
    width: 100%;
    height: 80%;

    display: flex;
    flex-wrap: wrap;

    h2 {
      font-size: 10px;
    }
  }

  .Contents {
    height: 50%;
    background-color: black;
    display: flex;
    align-items: center;

    color: white;
  }
  .Merchandise {
    height: 20%;
    background-color: #0282f9;
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

        img {
          height: 40px;
          width: 35px;
          vertical-align: middle;
          margin-right: 5px;
        }
      }
    }
  }

  .Item {
    position: relative;
    img {
      position: absolute;
      right: 10%;
      top: -12%;
      height: 450px;
      z-index: 0;
      transform: rotate(-25deg);
      opacity: 0.5;
    }

    height: 30%;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: top;
    display: flex;
    padding-top: 2rem;
    gap: 1rem;
    align-items: first baseline;
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
