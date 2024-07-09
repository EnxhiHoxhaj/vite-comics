<script>
import AppJumbo from './AppJumbo.vue'
export default {
    name: 'ProductGallery',
    components: {
        AppJumbo,
    }
}

</script>

<template>

    <section class="container">
        <div class="gallery">
            <AppJumbo/>
        </div> 
    </section>


</template>

<style lang="scss" scoped>

@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');

.container {

    background-color: black;
    
    

    .gallery {
        margin: 0 15rem;
        padding: 4rem 0;
        color: white;
    }
}

</style>