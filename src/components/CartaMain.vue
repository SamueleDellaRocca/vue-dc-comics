<template>
  <div>
    <div class="carta">
      <div class="immagine"><img :src="img" :alt="titolo" /></div>
      <div class="titolo">{{ titolo }}</div>
    </div>
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

<style scoped lang="scss"></style>
