<template>
    <div id="app">
        <!-- HEADER -->
        <Header />

        <!-- MAIN -->
        <Main />

        <!-- MAIN ICONS -->
        <Cards />
    </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Main from "@/components/Main.vue";
import Cards from "@/components/Cards.vue";

export default {
    name: "App",
    components: {
        Header,
        Main,
        Cards,
    },
};
</script>
  
<style lang="scss">
    @import './styles/general';
    @import './styles/utilities'; 
    @import './styles/vars'; 
</style>
