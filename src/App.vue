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
    },
    data () {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: true,                
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: false,               
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false,                
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,                
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false,                
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false,                
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false,               
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false,               
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false,               
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false,           
                }
            ]
        }  
    }
  }
</script>

<template>
  <header>
    <AppHeader :menuItems="links"/>
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
