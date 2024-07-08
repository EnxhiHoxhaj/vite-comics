<script>
export default {
    name: 'AppFooter',
    data () {
        return {
            button: 'SIGN UP NOW!',
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
    <footer>
        <section>
            <button> {{ button }}</button>
            <div class="right">
                <h3> {{ titleLink }}</h3>
                <div class="icone_social" v-for="(social, index ) in socials">
                    <img :src="social.icon" alt="">
                </div>
            </div>
        </section>
    </footer>

</template>
 
<style lang="scss" scoped>

@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');

footer {
    background-color: $geay_background;

    section {
        @include center('horizontal');
        justify-content: space-between;
        margin: 0 14rem;
        padding: 1.5rem 0;

        button {
            padding: 0.5rem;
            border-radius: 0;
            border-style: none;
            border:solid $light_text 0.1rem;
            background-color: transparent;

            &:hover {
                box-sizing: border-box;
                border-color: $primary
            }
        }

        .right {
            @include center('horizontal');
            gap: 1rem;
            font-family: "Bebas Neue", sans-serif;
            font-size: 1.2rem;
            color: $primary;

            .icone_social {
                width: 30px;

                img {
                    width: 100%;
                }
            }


        }
    }
}

</style>