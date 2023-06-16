<script>
import AppHeader from "./components/AppHeader.vue";
import AppJumbotron from "./components/AppJumbotron.vue"
import AppMain from "./components/AppMain.vue";
import AppFooter from "./components/AppFooter.vue";

export default{
  name: "App",
  components:{
    AppHeader,
    AppMain,
    AppJumbotron,
    AppFooter
  } 
  }
</script>

<template>
  <AppHeader />
  <AppJumbotron />
  <AppMain />
  <AppFooter />
</template>

<style lang="scss">
  @import "./styles/general.scss";
</style>
