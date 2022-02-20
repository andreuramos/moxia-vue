<template>
  <div class="overlay">
    <div class="dialog" v-bind:class="(hoveringOkButton)?'moixa-guaita':''">
      <div class="content">
        <span>{{ message }}</span>
      </div>
      <div class="dialog-buttons">
        <a
            class="button ok"
            @click="onOkClick()"
            @mouseenter="moixaGuaita()"
            @mouseleave="moixaAmaga()"
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
  data: function () {
    return {
      hoveringOkButton: false
    }
  },
  methods: {
    onOkClick () {
      this.$emit("ageVerification", true);
    },
    onKoClick () {
      this.$emit("ageVerification", false);
    },
    moixaGuaita() {
      this.hoveringOkButton = true;
    },
    moixaAmaga() {
      this.hoveringOkButton = false;
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
  z-index: 2;
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
  @keyframes saMoixaTeGuaita {
    from {background-position-y: -500px;}
    to {background-position-y: -250px;}
  }

  .moixa-guaita {
    background-image: url("../assets/moixa-guaita-1.png");
    background-repeat: no-repeat;
    background-position-x: calc(100% + 225px);
    background-position-y: -250px;
    animation-name: saMoixaTeGuaita;
    animation-duration: 1s;
  }

  .dialog {
    width: 30%;
  }
}
</style>
