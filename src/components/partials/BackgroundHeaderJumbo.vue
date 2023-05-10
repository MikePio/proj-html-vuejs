<script>
export default {
  name: 'BackgroundHeaderJumbo',
  data(){
    return{

    }
  }

}
</script>

<template>
  <div class="backgrounds-header-jumbo">
    <div class="backgrounds-header-jumbo-left"></div>
    <div class="backgrounds-header-jumbo-right"></div>
  </div>
</template>

<style lang="scss" scoped>
@use '../../scss/main.scss' as *;

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

</style>