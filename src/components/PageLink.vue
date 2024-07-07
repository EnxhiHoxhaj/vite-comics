<script>
export default {
    name: 'PageLink',
    data (){
        return {
            imgLink: [
                {
                    image: 'src/assets/buy-comics-digital-comics.png',
                    url: '#',
                    current: false,
                },
                {
                    image: 'src/assets/buy-comics-merchandise.png',
                    url: '#',
                    current: false,
                },
                {
                    image: 'src/assets/buy-comics-subscriptions.png',
                    url: '#',
                    current: false,
                },
                {
                    image: 'src/assets/buy-comics-shop-locator.png',
                    url: '#',
                    current: false,
                },
                {
                    image: 'src/assets/buy-dc-power-visa.svg',
                    url: '#',
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
                    <img :src="image.image" alt="">
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
}

</style>