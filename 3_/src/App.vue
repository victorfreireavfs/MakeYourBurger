<template>
    <div>
      <Navbar :logo="logo_src" :alt="app_name" id="logo_url"/>
      <router-view />
      <Footer />
    </div>
  </template>

<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'


export default {
  components:{
    Navbar,
    Footer
  },
  data(){
    return{
      logo_src:"/img/logo.png",
      app_name: "Make Your Burger"
    }
  }
}
</script>

<style>

</style>
