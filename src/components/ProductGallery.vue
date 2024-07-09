<script>
import AppJumbo from './AppJumbo.vue'
import AppOptions from './AppOptions.vue'
export default {
    name: 'ProductGallery',
    components: {
        AppJumbo,
        AppOptions
    }
}

</script>

<template>

    <section class="container">
        <div class="jumbo">
            <AppJumbo/>
        </div>
        <div class="gallery">
            <AppOptions/>
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