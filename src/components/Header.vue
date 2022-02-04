<template>
  <div id="header">
    <div id="logo-container">
      <img id="logo-text" src="../assets/logo.svg" alt="MOIXA"/>
      <img id="logo-img" src="../assets/moix-alpha-sm.png" alt="MOIXA"/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style>
  @import "../assets/styles/base.css";
  #navbar {

  }

  #header {
    background-color: var(--main-color);
    width: 100%;
  }

  #logo-container {
    margin: 0 auto;
    display: table;
    text-align: center;
    height: 10em;
    width: 60%;
  }

  #logo-text {
    display: inline-block;
    max-width: 70%;
    height: 10em;
  }

  #logo-img {
    display: inline-block;
    max-width: 30%;
    height: 10em;
  }
</style>
