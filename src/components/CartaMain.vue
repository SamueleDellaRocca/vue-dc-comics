<template>
  <div class="carta">
    <div class="immagine"><img :src="img" :alt="titolo" /></div>
    <div class="titolo">{{ titolo }}</div>
  </div>
</template>

<script>
export default {
  name: "CartaMain",
  props: {
    img: String,
    titolo: String,
  },
};
</script>

<style scoped lang="scss">
.carta {
  width: calc(100% / 6 - 1rem);
}

.immagine {
  margin-bottom: 10px;
  img {
    width: 100%;
  }
}

.titolo {
  color: white;
  text-transform: uppercase;
  font: 1.3rem;
}
</style>
