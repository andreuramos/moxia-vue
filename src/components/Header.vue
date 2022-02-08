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

  #header {
    background-color: var(--light-color);
    width: 100%;
  }

  #logo-container {
    margin: 0 auto;
    display: table;
    text-align: center;
    height: 5em;
    width: 100%;
  }

  #logo-text {
    display: inline-block;
    max-width: 70%;
    height: 5em;
    float: left;
  }

  #logo-img {
    display: inline-block;
    max-width: 29.5%;
    height: 5em;
    float: right;
    margin-right: 0.5%;
  }
</style>
