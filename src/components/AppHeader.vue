<script>
export default {
    name: 'AppHeader',
    data () {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: true,                
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: false,               
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false,                
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,                
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false,                
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false,                
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false,               
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false,               
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false,               
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false,           
                }
            ]
        }  
}
}
</script>

<template>
    <header>
        <nav>
            <div class="logo">
                <img src="../assets/dc-logo.png" alt="">
            </div>
            <!-- navigazione -->
            <ul>
                <li v-for="(linkHeader, index) in links" key="index">
                    <a :href="linkHeader.url" :class="linkHeader.current ? 'active' : ''">{{ linkHeader.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;
    @import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');


    header {
        nav {
            margin: 1.2rem 14rem;
            @include center('horizontal');
            justify-content: space-between;

            .logo {
            height: 70px;
            width: 100px;
            }

            img {
                height: 100%;
            }

            ul {

                @include center('vertical');
                gap: 1rem;
                
                li {
                    font-family: "Bebas Neue", sans-serif;
                    list-style: none;
                    font-weight:normal;
                    font-size: 0.9rem;

                    a {
                        text-decoration: none;
                        color:$text_color;
                        padding-bottom: 2.6rem;

                        &:hover, &.active{
                            border-bottom: solid $primary 0.3rem;
                        }

                    }
                }
            }

        }

    }

</style>