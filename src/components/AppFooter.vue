<script>
export default {
    name: 'AppFooter',
    data () {
        return {
            button: 'SIGN_UP NOW!',
            titleLink: 'FOLLOW US',
            socials: [
                {
                    icon:'src/assets/footer-facebook.png',
                },
                {
                    icon:'src/assets/footer-twitter.png',
                },
                {
                    icon:'src/assets/footer-youtube.png',
                },
                {
                    icon:'src/assets/footer-pinterest.png',
                },
                {
                    icon:'src/assets/footer-periscope.png',
                }
            ]
        }
    }
}

</script>

<template>


</template>
 
<style lang="scss" scoped>

@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');

</style>