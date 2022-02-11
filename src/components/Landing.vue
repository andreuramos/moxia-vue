<template>
  <div class="container">
    <div class="text-container">
      <p>
        <span class="main-text outline">Això era i no era</span>
      </p>
      <p>
        <span class="main-text outline">una</span>
        <span class="main-text">&nbsp;cervesa&nbsp;</span>
        <span class="main-text outline">mallorquina</span>
      </p>
      <p>
        <span class="main-text outline">de bon de veres</span>
      </p>
      <p>
        <span class="main-text">-moixa-</span>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Landing",
  data() {
    return {
      text: "Això era i no era una cervesa mallorquina de bon de veres."
    }
  }
}
</script>

<style>
@font-face {
  font-family: "Bourbon";
  src: url("../assets/BourbonSt-Regular.ttf");
}

.container {
  width: 100%;
}

.text-container {
  margin: 5% 15%;
  text-align: center;
}

.main-text {
  display: inline-block;
  font-family: Bourbon;
  text-transform: uppercase;
  font-size: 3em;
  color: var(--dark-color);
}

.outline {
  color: rgba(0,0,0,0%);
  -webkit-text-stroke: 1px black;
}

@media only screen and (min-width: 700px){
  .main-text {
    font-size: 8em;
  }
}
</style>
