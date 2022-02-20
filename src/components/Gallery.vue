<template>
  <section class="gallery">
    <img src="../assets/pictures/moixa-tronc.jpg"/>
    <img src="../assets/pictures/moixa-figuera.jpeg"/>
    <img src="../assets/pictures/moixa-marge.jpg"/>
  </section>
</template>

<script>
export default {
  name: "Gallery"
}
</script>

<style scoped>
.gallery {
  width: 100%;
  overflow-x: hidden;
}

.gallery img {
  position: absolute;
  width: 90%;
  padding: 5%;
}

@media only screen and (min-width: 700px) {
  .gallery img {
    position: relative;
    width: 30%;
    padding: 1.5%;
  }
}
</style>
