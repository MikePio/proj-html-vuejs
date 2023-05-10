<script>
import { store } from "./data/store"
import Header from './components/Header.vue'
import Jumbotron from './components/partials/Jumbotron.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

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
<div class="backgrounds-header-jumbo">
  <div class="backgrounds-header-jumbo-left"></div>
  <div class="backgrounds-header-jumbo-right"></div>
</div>
<div class="body-container d-flex flex-column align-items-center justify-content-center">
  <Header/>
  <Jumbotron/>
  <Main/>
  <Footer/>
</div>
</template>

<style lang='scss'>
@use './scss/main.scss' as *;
@import url('https://fonts.googleapis.com/css?family=Montserrat');
@import url('https://fonts.googleapis.com/css?family=Bai+Jamjuree');

body{
  color: white;
  background-color: $primary-color;
  // display: flex;
  // flex-direction: column;
  // align-items: center;
  // justify-content: center;
  //! NECESSARIA PER LO ZOOM ///////////////////////////////////////////////////////
  min-width: 1519px;

  .debug{
    border: 1px dashed blue;
  }

  //* TUTTI I BACKGROUND /////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////// 
  .backgrounds-header-jumbo{
    position: absolute;
    z-index: -1;
    display: flex;
    width: 100%;
    // width: 100vw;
    // height: 100vh;
    //*somma dell'altezza del jumbotron e del header
    height: 945px;
  }

  .backgrounds-header-jumbo-left {
    background-color: $primary-color;
    // // position: relative;
    // position: absolute;
    // top: 0;
    // left: 0;
    background-size: cover;
    // width: 28%;
    width: 29.5%;
    // width: 28vw;
    // width: 448px;
    height: 100%;
  }

  .backgrounds-header-jumbo-right {
    background-image: url("public/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg");
    background-size: cover;
    // background-position: center;
    // width: 72%;
    width: 70.5%;
    min-width: 1071px;
    // width: 72vw;
    // width: 1071px;
    height: 100%;
  }
  
  header, .jumbotron-mp{
    // position: relative;
    // z-index: 1;
  }

  //* TUTTI I COMPONENTS PRINCIPALI /////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////// 
  header, .jumbotron-mp, main, footer {
    // max-width: 1520px;
    // width: 1519px;
    min-width: 1519px;
  }





  .container-empty{
    // width: 100%;
    // min-width: 98vw;
  }

}

</style>
