<template>
  <section class="description">
    <img class="description-img" src="../assets/pictures/moixa-botella-sm.jpg" alt="botella de moixa">
    <div class="description-text-block">
    <p class="description-text">
        Moixa és una Cervesa Artesana amb caràcter mallorquí.
        Feta amb passió perque gaudim de fer cervesa, però sobre tot per a que gaudeixis tu bevent-la.
      </p>
      <p class="description-text">
        Fes el cap viu i tasta-la, perquè les millors històries són les que s'expliquen amb una cervesa a la mà.
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "Description"
}
</script>

<style scoped>
.description {
  width: 100%;
  margin-top: 2em;
  position: relative;
}

.description-img {
  position: absolute;
}

.description-text-block {
  position: absolute;
  right: 0;
  max-width: 60%;
  margin-top: 3em;
}

.description-text {
  font-style: italic;
  font-family: serif;
  float: right;
  font-size: larger;
}

@media only screen and (min-width: 700px) {
  .description-img {
    content: url("../assets/pictures/moixa-botella-lg.jpg");
    max-width: 60%;
  }
}
</style>
