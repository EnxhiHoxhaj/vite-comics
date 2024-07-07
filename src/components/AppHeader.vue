<script>
export default {
    name: 'AppHeader',
}
</script>

<template>
    <header>
        <nav>
            <div>
                <img src="../assets/dc-logo.png" alt="">
            </div>
            <!-- navigazione -->
            <ul>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                                <li>
                    <a href="#">CHARACTERS</a>
                </li>
                <li>
                    <a href="#">CHARACTERS</a>
                </li>

            </ul>
        </nav>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@use '../styles/general.scss' as *;

header {
    
    nav {
        @include center();
    }
}

</style>