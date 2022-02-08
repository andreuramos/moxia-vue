<template>
  <div id="app">
    <Header/>
    <Landing/>
  </div>
</template>

<script>
import Header from "./components/Header";
import Landing from "@/components/Landing";

export default {
  name: 'App',
  components: {
    Header, Landing
  }
}
</script>

<style>
 @import "assets/styles/base.css";
</style>
