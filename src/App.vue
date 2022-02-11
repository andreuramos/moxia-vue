<template>
  <div id="app">
    <Dialog
        message="Uep aqueix! Que ets major d'edat per agafar una moixa?"
        ok-button="Vés! Posa'men 3"
        ko-button="Batua, idoi no"
    />
    <Header/>
    <Landing/>
  </div>
</template>

<script>
import Header from "./components/Header";
import Landing from "@/components/Landing";
import Dialog from "@/components/Dialog";

export default {
  name: 'App',
  components: {
    Header, Landing, Dialog
  }
}
</script>

<style>
 @import "assets/styles/base.css";
</style>
