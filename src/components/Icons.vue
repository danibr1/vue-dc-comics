<template>
    <main>
        <div class="icons">
            
        </div>
    </main>
</template>

<script>
export default {
    name: 'Icons',
};
</script>

<style scoped lang="scss">
    main {
        background: #0282f9;
        height: 130px;
    }

   .icons {
        display: flex;
        justify-content: space-between;   
        font-size: 1.5rem;
        color: #fff;
        margin: 0 auto;
        width: 1170px;
   }

    /* per divedere lo spazio esatto  
    .cards {
        flex-basis: calc(100% /5);
    } */

</style>