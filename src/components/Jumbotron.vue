<script>
export default {
  name: 'Jumbotron',
  data(){
    return{

    }
  }

}
</script>

<template>
  <!-- <section class="debug jumbotron-mp"> -->
  <section class="debug jumbotron-mp d-flex flex-column justify-content-center">
    <!-- per fare la linea di lato usa ::before in css -->
    <h2 class="little-title">ALWATS THE BEST WAY YOU NEED IT</h2>
    <h1 class="big-title">THE BEST <br>BUSINESS <br>CONSULTING</h1>
    <div class="container-buttons d-flex align-items-end">
      <button>Read more</button>
      <div class="play-icon d-flex align-items-center justify-content-center">
        <i class="fas fa-play"></i>
      </div>
    </div>

  </section>

</template>

<style lang="scss" scoped>
@use '../scss/main.scss' as *;

//*JUMBOTRON
.jumbotron-mp{
  // height: calc(100vh - 82px);
  // height: 825px;
  height: 845px;
  padding: 0px 33px;
  // width: 100%;

  .little-title{
    font-family: montserrat,Sans-serif;
    font-size: 16px;
    font-weight: 400;
    letter-spacing: 2.8px;
    // margin: 0 0 15px 23px;
    // margin: 0 0 15px 72px;
    margin: 0 0 -5px 72px;
    position: relative;
    &::before{
      content: "";
      position: absolute;
      left: -71px;
      // bottom: 4px;
      bottom: 6px;
      width: 50px;
      height: 3px;
      margin: 13px 0 0;
      background-color: $light-green;
      // background-color: #39ffbf;
    }
  }
  .big-title{
    font-family: bai jamjuree,Sans-serif;
    font-size: 106px;
    font-weight: 700;
    line-height: 93px;
    margin-top: 37px;
  }
  .container-buttons{
    margin-top: 50px;

    button{
      font-family: montserrat,Sans-serif;
    text-transform: uppercase;
    border: none;
    // padding: 23px 57px;
    width: 227px;
    height: 64px;
    background-color: $light-green;
    text-shadow: 0 0 10px transparent;
      &:hover{
        background-color: $secondary-color;
        color: #fff;
      }
    }

    .play-icon {
      border-radius: 50%;
      width: 56px;
      height: 56px;
      border: 2px solid #fff;;
      margin: 0 39px;
      cursor: pointer;
    }

    & i {
      color: $light-green;
      font-size: 15px;
    }

  }


}

</style>