<script>
export default {
    name: 'AppHeader',
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
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">HOME</a>
                </li>
                <li>
                    <a href="#">ABCD</a>
                </li>
                <li>
                    <a href="#">ABC</a>
                </li>
                <li>
                    <a href="#">AB</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">HOME</a>
                </li>
                <li>
                    <a href="#">ABCD</a>
                </li>
                <li>
                    <a href="#">ABC</a>
                </li>
                <li>
                    <a href="#">AB</a>
                </li>

            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;

    @use '../styles/partials/mixins' as *;

    @use '../styles/general.scss' as *;

    @import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');


    header {
        nav {
            margin: 1rem 12rem;
            @include center('horizontal');
            justify-content: space-between;

            .logo {
            height: 60px;
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
                        padding: 1rem 0;
                        &:hover {
                            border-bottom: solid $primary 0.3rem;
                        }
                    }
                }
            }

        }

    }

</style>