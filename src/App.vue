<template>
  <div id="app">
    <!-- HEADER -->
    <Header />

    <!-- MAIN -->
    <Main />
    <!-- MAIN ICONS -->
    <Icons />

    
  </div>
</template>
<script>
import Header from "@/components/Header.vue";
import Main from "@/components/Main.vue";
import Icons from "@/components/Icons.vue";


export default {
  name: "App",
  components: {
    Header,
    Main,
    Icons,
  },
};
</script>
  
<style scoped>
  #app {
    font-family: 'Roboto Condensed', sans-serif;
  }
</style>
