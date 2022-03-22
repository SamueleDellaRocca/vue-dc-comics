<template>
  <footer>
    <div class="sfondo">
      <div class="container flexato">
        <div class="left-side">
          <ul class="lista-footer">
            <li><h3>Dc comics</h3></li>
            <li v-for="(link, index) in arrayDCComics" :key="index">
              <a href="">{{ link.text }}</a>
            </li>
          </ul>
        </div>

        <div class="right-side">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
    <div class="credits">
      <div class="container"></div>
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
}

.left-side,
.right-side {
  width: 50%;
}

.right-side img {
  width: 60%;
}

.credits {
  background-color: hsl(0deg 0% 19%);
  min-height: 200px;
}

.lista-footer {
  list-style: none;
  color: white;

  a {
    color: gray;
    text-decoration: none;
  }
}
</style>
