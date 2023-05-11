<script>
import { store } from "./data/store"
import BackgroundHeaderJumbo from "./components/partials/BackgroundHeaderJumbo.vue"
import Header from './components/Header.vue'
import Jumbotron from './components/Jumbotron.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components:{
    BackgroundHeaderJumbo,
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
  <BackgroundHeaderJumbo/>
  <div class="body-container d-flex flex-column align-items-center justify-content-center">
    <Header/>
    <Jumbotron/>
    <Main/>
    <Footer/>
  </div>
</template>

<style lang='scss'>
@use './scss/main.scss' as *;
// @import url('https://fonts.googleapis.com/css?family=Montserrat');
// @import url('https://fonts.googleapis.com/css?family=Bai+Jamjuree');
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Bai+Jamjuree:wght@200;300;400;500;600;700&display=swap');

body{
  color: white;
  background-color: $primary-color;
  // display: flex;
  // flex-direction: column;
  // align-items: center;
  // justify-content: center;
  //! NECESSARIA PER LO ZOOM ///////////////////////////////////////////////////////
  min-width: 1519px;

  // .debug{
  //   border: 0.5px dashed rgb(166, 255, 0);
  // }

  //* TUTTI I BACKGROUND /////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////// 
  header, .jumbotron-mp{
    // position: relative;
    // z-index: 1;
  }

  //* TUTTI I COMPONENTS PRINCIPALI /////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////// 
  header, .jumbotron-mp, main, footer {
    // max-width: 1520px;
    // max-width: 1519px;
    // width: 1519px;
    min-width: 1519px;
  }







}

</style>
