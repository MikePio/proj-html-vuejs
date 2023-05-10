<script>
import Header from '../components/Header.vue'
import Jumbotron from '../components/partials/Jumbotron.vue'
export default {
  name: 'HeaderAndJumbo',
  components:{
    Header,
    Jumbotron
  },
  data(){
    return{

    }
  }

}
</script>

<template>  




  <div>
    <!-- // TODO Creare UN DIV un background di colore blu e poi inserire l'immagine con background-position: top right; -->
    <!-- <div class="container"> -->
      <!-- <div class="right"></div> -->
      <!-- <img src="public/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg" alt="img-background"> -->
    <!-- </div> -->
    <div class="background">
      <div class="left"></div>
      <div class="right"></div>
    </div>
      <Header/>
      <Jumbotron/>
    <!-- <div class="background">
      <Header/>
      <Jumbotron/>
      <div class="img-background"></div>
    </div> -->
  </div>


</template>

<style lang="scss" scoped>
@use '../scss/main.scss' as *;

.background {
  position: absolute;
  z-index: -1;
  display: flex;
  width: 100%;
  // width: 100vw;
  // height: 100vh;
  //*somma dell'altezza del jumbotron e del header
  height: 947px;

}

.left {
  background-color: $primary-color;
  // // position: relative;
  // position: absolute;
  // top: 0;
  // left: 0;
  background-size: cover;
  width: 28vw;
  // width: 28%;
  // width: 448px;
  height: 100%;
}

.right {
  background-image: url("public/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg");
  background-size: cover;
  // background-position: center;
  width: 72vw;
  // width: 72%;
  // width: 1071px;
  height: 100%;
}

header, .jumbotron-mp{
  // position: relative;
  // z-index: 1;
}


</style>