<template>
  <div class="text-container">
    <p class="main-text">
      {{ text }}
    </p>
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

.text-container {
  margin: 15%;
}

.main-text {
  font-family: Bourbon;
  text-transform: uppercase;
  font-size: xxx-large;
  color: var(--dark-color);
  text-align: center;
}
</style>
