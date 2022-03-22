<template>
  <footer>
    <div class="sfondo">
      <div class="container flexato">
        <div class="left-side">
          <div>
            <ul class="lista-footer">
              <li><h3>DC COMICS</h3></li>
              <li v-for="(link, index) in arrayDCComics" :key="index">
                <a href="">{{ link.text }}</a>
              </li>
            </ul>

            <ul class="lista-footer">
              <li><h3>SHOP</h3></li>
              <li v-for="(link, index) in arrayShop" :key="index">
                <a href="">{{ link.text }}</a>
              </li>
            </ul>
          </div>

          <div>
            <ul class="lista-footer">
              <li><h3>DC</h3></li>
              <li v-for="(link, index) in arrayDC" :key="index">
                <a href="">{{ link.text }}</a>
              </li>
            </ul>
          </div>

          <div>
            <ul class="lista-footer">
              <li><h3>SITES</h3></li>
              <li v-for="(link, index) in arraySites" :key="index">
                <a href="">{{ link.text }}</a>
              </li>
            </ul>
          </div>
        </div>

        <div class="right-side">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
    <div class="credits">
      <div class="container flex">
        <div class="credits-left">
          <button>SIGN-UP NOW!!</button>
        </div>

        <div class="credits-right">
          <h3>FOLLOW US</h3>
          <div><img src="../assets/img/footer-facebook.png" alt="" /></div>
          <div><img src="../assets/img/footer-twitter.png" alt="" /></div>
          <div><img src="../assets/img/footer-youtube.png" alt="" /></div>
          <div><img src="../assets/img/footer-pinterest.png" alt="" /></div>
          <div><img src="../assets/img/footer-periscope.png" alt="" /></div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterDCcomics",
  data() {
    return {
      arrayDCComics: [
        {
          text: "Characters",
        },
        {
          text: "Comics",
        },
        {
          text: "Movies",
        },
        {
          text: "TV",
        },
        {
          text: "Games",
        },
        {
          text: "Videos",
        },
        {
          text: "News",
        },
      ],

      arrayShop: [
        {
          text: "Shop DC",
        },
        {
          text: "Shop DC Collectibles",
        },
      ],

      arrayDC: [
        {
          text: "Terms Of Use",
        },
        {
          text: "Privacy policy(New)",
        },
        {
          text: "Ad Choises",
        },
        {
          text: "Advertising",
        },
        {
          text: "Jobs",
        },
        {
          text: "Subscriptions",
        },
        {
          text: "Talent Workshops",
        },
        {
          text: "CPSC Certificates",
        },
        {
          text: "Ratings",
        },
        {
          text: "Shop Help",
        },
        {
          text: "Contact Us",
        },
      ],

      arraySites: [
        {
          text: "DC",
        },
        {
          text: "MAD Magazine",
        },
        {
          text: "DC Kids",
        },
        {
          text: "DC Universe",
        },
        {
          text: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.sfondo {
  background-image: url(../assets/img/footer-bg.jpg);
}

.container {
  width: 80%;
  margin: auto;
}

.flexato {
  display: flex;
  height: 400px;
  overflow: hidden;
  padding: 1rem 0px;
}

.left-side {
  display: flex;
  width: 70%;
  gap: 2rem;
}

.right-side img {
  width: 100%;
}

.credits {
  background-color: hsl(0deg 0% 19%);
}

.lista-footer {
  list-style: none;
  color: white;
  margin-top: 2rem;

  li {
    padding: 3px 0px;
  }

  a {
    color: gray;
    text-decoration: none;
  }
}

.flex {
  display: flex;
  align-items: center;
  padding: 1rem;
}

.credits-left {
  width: 65%;
  button {
    padding: 10px 15px;
    background-color: transparent;
    border: 2px solid hsl(211deg 91% 50%);
    color: white;
    cursor: pointer;
  }
}

.credits-right {
  width: 35%;
  display: flex;
  align-items: center;
  gap: 15px;

  h3 {
    color: hsl(211deg 91% 50%);
    cursor: pointer;
  }

  div {
    cursor: pointer;
  }
}
</style>
