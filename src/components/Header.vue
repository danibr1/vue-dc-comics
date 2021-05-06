<template>
    <!-- HEADER -->
    <header class="container">
        <!-- HOME LOGO -->
        <a :href="logo.url">
            <img :src="logo.image" :alt="logo.text" />
        </a>
        <!-- NAVBAR -->
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a 
                        href="link.url">{{ link.text }}
                    </a>
                </li>

                
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: "Header",
    data () {
        return {
            logo: {
                image: require('@/assets/img/dc-logo.png'),
                url: '/',
                text: 'DC logo',
            },
            
            links: [
                { text: 'character', url: '/character', current: false},
                { text: 'comics', url: '/comics', current: false},
                { text: 'movie', url: '/movie', current: false},
                { text: 'tv', url: '/tv', current: false},
                { text: 'games', url: '/games', current: false},
                { text: 'collectibles', url: '/collectibles', current: false},
                { text: 'videos', url: '/videos', current: false},
                { text: 'fans', url: '/fans', current: false},
                { text: 'news', url: '/news', current: false},
                { text: 'shop', url: '/shop', current: false},
            ]
        }
    },
};
</script>

<style scoped lang="scss">
    @import '../styles/vars';

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 115px;
}
img {
    height: 80px;
}

nav {
    ul {
        display: flex;
        list-style: none;
    }
}
li{
    a {
        font-size: 12px;
        font-weight: 700;
        text-decoration: none;
        text-transform: uppercase;
        padding: 45px 15px;
        color: #4b4e62;
        &:hover{
            color: $primary;
            border-bottom: 4px solid $primary;
        }
    }
}
.active {
    color: $primary;
    border-bottom: 4px solid $primary;
}
</style>