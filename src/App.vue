<script>
import { store } from "./data/store"
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import Jumbotron from './components/partials/Jumbotron.vue'
export default {
  name: 'App',
  components:{
    Header,
    Jumbotron,
    Main,
    Footer
  },
  data(){
    return{
      store
    }
  }
}
</script>

<template>
  <Header/>
  <Jumbotron/>
  <Main/>
  <Footer/>
</template>

<style lang='scss'>
@use './scss/main.scss' as *;
@import url('https://fonts.googleapis.com/css?family=Montserrat');
@import url('https://fonts.googleapis.com/css?family=Bai+Jamjuree');

body{
  color: white;
  background-color: rgb(37, 32, 32);

  .debug{
    border: 1px dashed blue;
  }

}

</style>
