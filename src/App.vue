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
  
<style lang="scss">
    @import './styles/general';
    @import './styles/utilities'; 
    @import './styles/vars'; 
</style>
