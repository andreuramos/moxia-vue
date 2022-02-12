<template>
  <div class="overlay">
    <div class="dialog">
      <div class="content">
        <span>{{ message }}</span>
      </div>
      <div class="dialog-buttons">
        <a
            class="button ok"
            @click="onOkClick()"
        >{{ okButton }}</a>
        <a
            v-if="koButton"
            class="button ko"
            @click="onKoClick()"
        >{{ koButton }}</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Dialog",
  props: ["message", "okButton", "koButton"],
  methods: {
    onOkClick () {
      this.$emit("ageVerification", true);
    },
    onKoClick () {
      this.$emit("ageVerification", false);
    }
  }
}
</script>

<style scoped>
.overlay {
  background-color: rgba(2,2,2,60%);
  position: absolute;
  width: 100%;
  height: 100%;
}

.dialog {
  position: relative;
  margin: 0 auto;
  width: 80%;
  background-color: var(--main-color);
  top: 50%;
  transform: translateY(-50%);
  font-family: Moderat;
  font-size: larger;
}

.content {
  display: block;
  padding: 2em;
}

.dialog-buttons {
  display: block;
  padding: 1em;
}

.button {
  display: inline-block;
  margin: 0.5em;
}

@media only screen and (min-width: 700px) {
  .dialog {
    width: 30%;

    background-image: url("../assets/moixa-guaita-1.png");
    background-repeat: no-repeat;
    background-position-x: calc(100% + 250px);
    background-position-y: -250px;
  }
}
</style>
