<template>
  <section>
    <div class="story">
      <div class="story-block">
        <p class="story-text">
          Això era i no era una Moixa dolenta, mentidera, més viva que el Dimoni i ben punyetera.
        </p>
      </div>
      <div class="story-block">
        <p class="story-text">
          Obrir una Moixa és jugar amb sa temptació. És saber que t'està mirant però ignorar-la. Tranquil, ho tens tot controlat.
        </p>
        <p class="story-text">
          Es problema és que no saps ni com, ja has obert sa tercera i vas calent de cap.
        </p>
        <p class="story-text">
          Ja està. Ja te té.
        </p>
        <p class="story-text">
          Sa Moixa se t'enduu.
        </p>
      </div>
      <div class="story-block story-picture-block">
        <img class="story-picture" src="../assets/moix-alpha-sm.png"/>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Story"
}
</script>

<style scoped>
.story {
  width: 100%;
  display: block;
}

.story-block {
  width: 70%;
  margin-left: 15%;
  margin-right: 15%;
}

.story-text {
  padding: 1em;
  font-family: Montserrat;
  text-transform: uppercase;
}

.story-picture {
  height: 60%;
  vertical-align: bottom;
}

.story-picture-block {
  display: flex;
  align-items: flex-end;
  justify-content: flex-end;
}

@media only screen and (min-width: 700px) {
  .story {
    display: flex;
  }


  .story-block {
    width: 30%;
    margin-left: 0;
    margin-right: 0;
  }
}
</style>
