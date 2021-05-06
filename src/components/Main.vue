<template>
    <main>
        <div class="content container">
            Content goes here
        </div>
    </main>
</template>

<script>
export default {
    name: 'Main',
};
</script>

<style scoped lang="scss">
    @import '../styles/general';
    @import '../styles/mixins';
    @import '../styles/utilities';
    @import '../styles/vars';

    main {
        background: #1c1c1c;
    }

   .content {
        font-size: 1.5rem;
        color: #fff;
        padding: 45px 0;
   }
</style>
    