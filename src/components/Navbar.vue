<template>
  <div id="navbar">
    <div id="header" class="debug">
      <div id="logo-container" class="debug">
        <img class="logo" src="../assets/logo.svg"/>
        <img class="logo" src="../assets/moix-alpha-sm.png"/>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navbar'
}
</script>

<style>
  @import "../assets/styles/base.css";
  #navbar {
    background-color: var(--main-color);
    width: 100%;
  }

  #header {
    margin: 0 auto;
    width: 60%;
  }

  #logo-container {
    margin: 0 auto;
    display: table;
    text-align: center;
    height: 10em;
  }

  .logo {
    display: inline-block;
    max-width: 50%;
    height: 10em;
  }
</style>
