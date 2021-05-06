<template>
    <main class="ai-center">
        <section class="container">
            <ul>
                <li  
                    v-for="(card, index) in cards" 
                    :key="index"
                    class="ai-center"
                >
                    <a :href="card.url">
                        <img :src="card.image" :alt="card.name">
                        <span>{{ card.name }}</span>
                    </a>
                </li>
            </ul>
        </section>
    </main>
</template>


<script>
export default {
    name: 'Cards',
    data() {
        return {
            cards: [
                {
                    name: 'Digital Comics',
                    url: '/digitalcomics',
                    image: require('@/assets/img/buy-comics-digital-comics.png')
                },
                {
                    name: 'DC Merchandise',
                    url: '/dcmerchandise',
                    image: require('@/assets/img/buy-comics-merchandise.png')
                },
                {
                    name: 'Subscription',
                    url: '/subscription',
                    image: require('@/assets/img/buy-comics-subscriptions.png')
                },
                {
                    name: 'Comic Shop Locator',
                    url: '/comicshoplocator',
                    image: require('@/assets/img/buy-comics-shop-locator.png')
                },
                {
                    name: 'DC Power Visa',
                    url: '/dcpowervisa',
                    image: require('@/assets/img/buy-dc-power-visa.svg')
                },
            ]
        }
    }
};
</script>


<style scoped lang="scss">
    @import '../styles/general';
    @import '../styles/mixins';
    @import '../styles/utilities';
    @import '../styles/vars';

    main {
        height: 150px;
        background: #0282f9;
    }

    ul{
        display: flex;
        justify-content: space-around;
    }
    li {
        list-style: none;
        margin: 0 15px;
        text-transform: uppercase;
        &:last-child{
            margin-right: 0;
        }
    }

    a{
        color: #fff;
        text-decoration: none;
    }

    img{
        height: 55px;
        margin-right: 10px;
        vertical-align: middle;
    }
    
    li:last-child img{
        width: 55px;
    }

    span {
        font-size:14px;
    }
</style>