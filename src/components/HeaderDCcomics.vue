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
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: space-between;

  img {
    padding: 1rem 0px;
  }
}

.ul-nav li {
  display: inline-block;
  padding: 48.5px 1rem;
  border-bottom: 10px solid transparent;
  margin-bottom: -10px;

  a {
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    color: black;
  }

  &:hover {
    color: rgb(2 130 249);
    border-bottom: 10px solid rgb(2 130 249);
  }

  &:hover a {
    color: rgb(2 130 249);
  }
}
</style>
