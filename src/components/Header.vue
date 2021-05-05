<template>
  <header>
       <a href="">
           <img src="../assets/img/dc-logo.png" alt="">
       </a>

       <nav>
            <a href="#">character</a>
            <a href="#">comics</a>
            <a href="#">movies</a>
            <a href="#">tv</a>
            <a href="#">games</a>
            <a href="#">collectibles</a>
            <a href="#">videos</a>
            <a href="#">fans</a>
            <a href="#">news</a>
            <a href="#">shop</a>
       </nav>
</header>
</template>

<script>
export default {
    name: 'Header',
};
</script>

<style scoped>
    header { 
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin: 0 auto;
        width: 1170px;
    }
    img {
        height: 70px;
    }
    nav a {
        color: #4b4e62;
        text-decoration: none;
        display: inline-block;
        text-transform: uppercase;
        font-size: 12px;
        font-weight: 700;
        padding: 45px 15px;
        border-bottom: 4px solid transparent;
    }

    nav a:hover{
        content:'';
        color: #0282f9;
        border-bottom: 4px solid #0282f9;
    }
</style>