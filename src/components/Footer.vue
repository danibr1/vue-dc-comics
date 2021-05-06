<template>
    <main>
        <!-- TOP FOOTER -->
        <section class="top-footer">
            <div class="container">
                
            </div>    
        </section>

        <section class="bottom-footer">
            <div class="container">
                
            </div>    
        </section>
    </main>
</template>


<script>
export default {
    name: 'Footer',
    data() {
        return {
           
        }
    }
};
</script>


<style scoped lang="scss">
    @import '../styles/general';
    @import '../styles/mixins';
    @import '../styles/utilities';
    @import '../styles/vars';

    // TOP FOOTER
    .top-footer {
        height: 370px;
        background: #5e5e5e;
    }

    // BOTTOM-FOOTER
    .bottom-footer {
        height: 110px;
        background: #2e2d2d;
    }
</style>