<template>
  <section>
    <div class="container">
      <img id="landing-img" src="../assets/landing-sm.svg" alt="Cervesa Artesana de Mallorca"/>
      <img id="dolentia-seal" src="../assets/feta-dolentia.svg"/>
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
  right:0%;
}

@media only screen and (min-width: 700px){
  #landing-img {
    content: url("../assets/landing-lg.svg");
  }

  #dolentia-seal {
    top: 65%;
    right: 15%;
  }
}
</style>
