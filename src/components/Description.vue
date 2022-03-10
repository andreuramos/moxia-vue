<template>
  <section class="description">
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

.description-text-block {
  right: 0;
  margin-top: 3em;
  background-image: url("../assets/pictures/moixa-botella-sm.jpg");
  background-position-y: center;
  background-repeat: no-repeat;
  padding-top: 10em;
  padding-bottom: 10em;
}

.description-text {
  margin-top: 2em;
  padding-left: 60%;
  font-style: italic;
  font-family: serif;
  font-size: larger;
}

@media only screen and (min-width: 700px) {
  .description-text-block {
    background-image: url("../assets/pictures/moixa-botella-lg.jpg");
  }
}
</style>
