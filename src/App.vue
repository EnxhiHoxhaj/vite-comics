<script>
import AppHeader from './components/AppHeader.vue'
import ProductGallery from './components/ProductGallery.vue'
import PageLink from './components/PageLink.vue'
import AppInfo from './components/AppInfo.vue'
import AppFooter from './components/AppFooter.vue'
export default {
  name: 'App',
  components: {
    AppHeader,
    ProductGallery,
    PageLink,
    AppInfo,
    AppFooter,
  }
}
</script>

<template>
  <AppHeader/>
  <main>
    <ProductGallery/>
    <PageLink/>
    <AppInfo/>
  </main>
  <AppFooter/>
</template>

<style lang="scss">
@use './styles/general.scss' as *;

</style>
