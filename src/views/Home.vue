<template>
  <header>
    <div class="logo">
      <router-link to="/" class="router"><img src="..\images\logo.svg" alt="Logo"></router-link>
      
    </div>

  </header>
  <Body/>
  <Footer/>

</template>

<script>
// @ is an alias to /src
import Body from '../components/Body'
import Footer from '../components/Footer'

export default {
  name: 'Home',
  components:{
    Body,
    Footer,
 
  }
}
</script>

<style>
  header{
    margin-top: 4em;
    margin-left: 4em;

  }
  header .logo{
    width: auto;
    height: 5em;
    position: relative;
  }
  header .logo img{
    width: 14em;
  }
</style>
