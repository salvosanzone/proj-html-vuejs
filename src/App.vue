<template>
  <div>  
    <Header 
      :menu="menuHeader"
    />
    <Main />
    <Footer 
      :avadaMovers="avadaMoversList" 
      :recentPosts="recentPostsList"
    />
  </div>

</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import menuHeader from './assets/data/menuHeader.js'
import avadaMoversList from './assets/data/avadaMoversList.js'
import recentPostsList  from './assets/data/recentPostsList.js'


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer

  },
  data(){
    return {
      //creo tre array che invio tramite le props
      menuHeader,
      avadaMoversList,
      recentPostsList 
    }
  }
}
</script>

<style lang="scss">
  @import'./assets/style/vars.scss';
  @import'./assets/style/general.scss';
</style>
