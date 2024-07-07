<script>
import AppHeader from './components/AppHeader.vue'
import ProductGallery from './components/ProductGallery.vue'
import PageLink from './components/PageLink.vue'
import AppInfo from './components/AppInfo.vue'
import Footer from './components/Footer.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    ProductGallery,
    PageLink,
    AppInfo,
    Footer
  }
}
</script>

<template>
  <AppHeader/>
  <ProductGallery/>
  <PageLink/>
  <AppInfo/>
  <Footer/>
</template>

<style lang="scss">
@use './styles/general.scss' as *;

</style>
