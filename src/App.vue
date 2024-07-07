<script>
import AppHeader from './components/AppHeader.vue'
import ProductGallery from './components/ProductGallery.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    ProductGallery,
  }
}
</script>

<template>
  <AppHeader/>
  <ProductGallery/>
</template>

<style lang="scss">
@use './styles/general.scss' as *;

</style>
