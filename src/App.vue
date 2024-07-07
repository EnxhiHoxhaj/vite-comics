<script>
import AppHeader from './components/AppHeader.vue'
import ProductGallery from './components/ProductGallery.vue'
import PageLink from './components/PageLink.vue'
import AppInfo from './components/AppInfo.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    ProductGallery,
    PageLink,
    AppInfo
  }
}
</script>

<template>
  <AppHeader/>
  <ProductGallery/>
  <PageLink/>
  <AppInfo/>
</template>

<style lang="scss">
@use './styles/general.scss' as *;

</style>
