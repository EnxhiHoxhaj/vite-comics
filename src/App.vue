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
  <header>
    <AppHeader/>
  </header>

  <main>
    <ProductGallery/>
    <PageLink/>
  </main>

  <footer>
    <AppInfo/>
    <AppFooter/>
  </footer>

</template>

<style lang="scss">
@use './styles/general.scss' as *;
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');

</style>
