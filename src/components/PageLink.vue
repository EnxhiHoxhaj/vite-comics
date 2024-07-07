<script>
export default {
    name: 'PageLink',
    data (){
        return {
            imgLink: [
                {
                    image: 'src/assets/buy-comics-digital-comics.png',
                    url: '#',
                    text: 'DIGITAL COMICS',
                    current: false,
                },
                {
                    image: 'src/assets/buy-comics-merchandise.png',
                    url: '#',
                    text: 'DC MERCHANDISE',
                    current: false,
                },
                {
                    image: 'src/assets/buy-comics-subscriptions.png',
                    url: '#',
                    text: 'SUBSCRIPTION',
                    current: false,
                },
                {
                    image: 'src/assets/buy-comics-shop-locator.png',
                    url: '#',
                    text: 'COMICS SHOP LOCATOR',
                    current: false,
                },
                {
                    image: 'src/assets/buy-dc-power-visa.svg',
                    url: '#',
                    text: 'DC POWER VISA',
                    current: false,
                },
            ]
        }
    }
}

</script>

<template>
        <div class="container">
            <ul>
                <li v-for="(image, index) in imgLink" key="index">
                    <div class="icone">
                        <img :src="image.image" alt="">
                    </div>
                    <div>
                        <a href="#"> {{ image.text }}</a>
                    </div>
                </li>
            </ul>
        </div>
</template>

<style lang="scss" scoped>

@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');

.container {
    background-color: $primary;
    padding: 2rem 17rem;

    ul {
        @include center('horizontal');
        justify-content: space-between ;
        
        li {
            list-style: none;
            @include center();
            gap: 1rem;
            
            .icone {
                width: 40px;
            }
            
            img {
                width: 100%;
            }

            a {
                text-decoration: none;
                font-size: 0.7rem;
                color: white;
            }
        }
    }
}

</style>