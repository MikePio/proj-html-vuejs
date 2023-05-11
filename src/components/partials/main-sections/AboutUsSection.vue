<script>
export default {
  name: 'AboutUsSection',
  data(){
    return{

    }
  }

}
</script>

<template>
  <section class="debug about-us-section">

  <!--//* big-container -->
    <div class="big-container d-flex">
      <div class="big-container-left"></div>
      <div class="big-container-right d-flex flex-column justify-content-center align-items-start">
        <p>ABOUT US</p>
        <h3>WE MAKE YOUR<br> STRATEGY WORK</h3>
        <p class="description-big-container m-0">When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed when I hear the buzz of the little world among the stalks,and grow familiar indescribable forms of the insects .and flies, then I feel the presence of the Almighty .</p>
      </div>

    </div>

  <!--//* little-container -->
    <div class="little-container">

    </div>
  </section>

</template>

<style lang="scss" scoped>
@use '../../../scss/main.scss' as *;

.about-us-section{
  
  .big-container{
    height: 560px;
    // width: 100%;
  }
  .big-container-left{
    width: 58%;
    background-image: url('public/images/business-people-working-together-on-project-and-5FHSKBL.jpg');
    background-size: cover;
  }
  .big-container-right{
    margin-left: 60px;

    p{
      font-family: montserrat,Sans-serif;
      font-size: 16px;
      font-weight: 400;
      line-height: 19px;
      letter-spacing: 2.8px;
      color: white;
      margin: 0 0 15px 23px;
      position: relative;
      &:first-child{
        margin-left: 70px;
      }
      &:first-child::before{
        content: "";
        height: 3px;
        margin: 13px 0 0;
        background-color: $light-green;
        position: absolute;
        left: -71px;
        bottom: 6px;
        width: 50px;
      }
    }
    h3{
      font-family: bai jamjuree,Sans-serif;
      font-size: 60px;
      font-weight: 700;
      line-height: 65px;
    }
    .description-big-container{
      color: rgba(255,255,255,.6);
      font-family: montserrat,Sans-serif;
      font-size: 16px;
      font-weight: 400;
      line-height: 25px;
      letter-spacing: 0;
      max-width: 498px;
    }
  }
  .little-container{
    height: 325px;
    background-color: $light-green;
    margin-right: 1.18%;
  }

}


</style>