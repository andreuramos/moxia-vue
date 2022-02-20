<template>
  <section>
    <div class="container">
      <img id="landing-img" src="../assets/landing-sm.svg" alt="Cervesa Artesana de Mallorca"/>
      <img id="dolentia-seal" src="../assets/feta-dolentia.svg"/>
      <img id="landing-brand" src="../assets/brand-hyphens.svg"/>
    </div>
  </section>
</template>

<script>
export default {
  name: "Landing"
}
</script>

<style>
.container {
  width: 100%;
}

#landing-img {
  content:url("../assets/landing-sm.svg");
  width: 90%;
  margin: 5%;
}

#dolentia-seal {
  position: fixed;
  display: block;
  top: 40%;
  right: 5%;
  z-index: 1;
}

#landing-brand {
  width: 60%;
  margin-top: 10%;
  margin-left: 20%;
  margin-right: 20%;
}

@media only screen and (min-width: 700px){
  #landing-img {
    content: url("../assets/landing-lg.svg");
  }

  #dolentia-seal {
    top: 65%;
    right: 15%;
  }

  #landing-brand {
    width: 40%;
    margin-top: 5%;
    margin-left: 30%;
  }
}
</style>
