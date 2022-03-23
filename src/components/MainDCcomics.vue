<template>
  <main>
    <div class="black">
      <div class="container">
        <h1>--> Content goes here &lt;--</h1>
      </div>
    </div>

    <div class="blu">
      <div class="container">
        <ul class="list-main">
          <li v-for="(link, index) in arrayLinkMain" :key="index">
            <a href="">
              <img
                :src="require('../assets/img/' + link.img)"
                :alt="link.text"
              />
              {{ link.text }}
            </a>
          </li>
        </ul>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainDCcomics",
  data() {
    return {
      arrayLinkMain: [
        {
          text: "digital comics",
          img: "buy-comics-digital-comics.png",
        },
        {
          text: "dc merchandise",
          img: "buy-comics-merchandise.png",
        },
        {
          text: "subscription",
          img: "buy-comics-subscriptions.png",
        },
        {
          text: "comic shop locator",
          img: "buy-comics-shop-locator.png",
        },
        {
          text: "dc power visa",
          img: "buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}
.container {
  width: 80%;
  margin: auto;

  h1 {
    color: white;
    padding: 3rem;
  }
}

.blu {
  background-color: rgb(2 130 249);
}

.black {
  background-color: black;
}

.list-main {
  display: flex;
  li {
    display: flex;
    align-items: center;
    padding: 2rem 0px;

    img {
      width: 20%;
      object-fit: contain;
      margin-right: 10px;
    }

    a {
      text-decoration: none;
      color: white;
      text-transform: uppercase;
      display: flex;
      align-items: center;
    }
  }
}
</style>
