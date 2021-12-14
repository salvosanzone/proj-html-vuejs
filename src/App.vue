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
      menuHeader: [
        {
          name: 'Home',
          id: 1,
          actived: true
        },
        {
          name: 'Rates',
          id: 2,
          aactived: false
          
        },
        {
          name: 'Testimonials',
          id: 3,
          actived: false
        },
        {
          name: 'FAQ',
          id: 4,
          actived: false
        },
        {
          name: 'Blog',
          id: 5,
          actived: false
        },
        {
          name: 'Contact',
          id: 6,
          actived: false
        },
      ],
      avadaMoversList: [
        {
          name: 'Home',
          id: 1,
          actived: true
        },
        {
          name: 'Rates',
          id: 2,
          actived: false
        },
        {
          name: 'Testimonials',
          id: 3,
          actived: false
        },
        {
          name: 'Blog',
          id: 4,
          actived: false
        },
        {
          name: 'Free Quote',
          id: 5,
          actived: false
        },
      ],
      recentPostsList: [
        {
          name: 'Heading Out To College?',
        },
        {
          name: 'Moving Your Business?',
        },
        {
          name: 'Outstanding Quality',
        },
        {
          name: 'Cost Of Moving',
        },
        {
          name: 'Best Moving Tips',
        },
      ]
    }
  }
}
</script>

<style lang="scss">
  @import'./assets/style/vars.scss';
  @import'./assets/style/general.scss';
</style>
