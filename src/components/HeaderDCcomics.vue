<template>
  <header>
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="logo dc" />
      <ul class="ul-nav">
        <li v-for="(li, index) in arrayLinkNav" :key="index">
          <a href="">{{ li.text }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderDCcomics",
  data() {
    return {
      arrayLinkNav: [
        {
          text: "characters",
        },
        {
          text: "comics",
        },
        {
          text: "movies",
        },
        {
          text: "tv",
        },
        {
          text: "games",
        },
        {
          text: "collectibles",
        },
        {
          text: "videos",
        },
        {
          text: "fans",
        },

        {
          text: "news",
        },
        {
          text: "shop",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
.container {
  width: 80%;
  padding: 1rem 0px;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.ul-nav li {
  display: inline-block;
  padding: 1rem;

  a {
    text-decoration: none;
    text-transform: uppercase;
    color: black;
    font-weight: bold;
  }
}
</style>
