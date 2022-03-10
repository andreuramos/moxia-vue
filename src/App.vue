<template>
  <div id="app">
    <Dialog
        v-if="!isAgeVerified"
        message="Uep aqueix! Que ets major d'edat per agafar una bona moixa?"
        ok-button="Vés! Posa'men 3"
        ko-button="Batua, idoi no"
        @ageVerification="handleAgeVerification"
    />
    <Header/>
    <Landing/>
    <Gallery/>
    <Description/>
    <Story/>
  </div>
</template>

<script>
import Header from "./components/Header";
import Landing from "@/components/Landing";
import Dialog from "@/components/Dialog";
import Gallery from "@/components/Gallery";
import Description from "@/components/Description";
import Story from "@/components/Story";

export default {
  name: 'App',
  components: {
    Story,
    Description,
    Gallery,
    Header, Landing, Dialog
  },
  data: function() {
    return {
      'isAgeVerified': false
    }
  },
  methods: {
    handleAgeVerification (result) {
      if (result) {
        this.isAgeVerified = true;
      } else {
        window.location.href = "https://www.google.com"
      }
    }
  }
}
</script>

<style>
 @import "assets/styles/base.css";
</style>
