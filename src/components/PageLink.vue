<script>
export default {
    name: 'PageLink',
    data (){
        return {
            imgLink: [
                {
                    image: 'src/assets/buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS',
                },
                {
                    image: 'src/assets/buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE',
                },
                {
                    image: 'src/assets/buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION',
                },
                {
                    image: 'src/assets/buy-comics-shop-locator.png',
                    text: 'COMICS SHOP LOCATOR',
                },
                {
                    image: 'src/assets/buy-dc-power-visa.svg',
                    text: 'DC POWER VISA',
                },
            ]
        }
    }
}

</script>

<template>
        <section class="container">
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
        </section>
</template>

<style lang="scss" scoped>

@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');

.container {
    background-color: $primary;
    padding: 2rem 18rem;

    ul {
        @include center('horizontal');
        justify-content: space-between ;
        li {
            font-weight: bold;
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