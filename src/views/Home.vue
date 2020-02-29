<template>
  <div class="home" >
    <WTMHome />
    <v-container class="spacing-playground  google-font" >
      <AboutWTM />
      <WTMAddis /> 
      <Events />
      <Partners /> 
    </v-container>
    <Footer />
  </div>
</template>

<script>
import WTMHome from "../components/WTMHome";
import AboutWTM from "../components/AboutWTM";
import WTMAddis from "../components/WTMAddis";
import Events from "../components/Events";
import Partners from "../components/Partners";
import Footer from "../components/Footer";
export default {
  components: {
    WTMHome,
    AboutWTM,
    WTMAddis,
    Events,
    Partners,
    Footer,
  }
};
</script>
