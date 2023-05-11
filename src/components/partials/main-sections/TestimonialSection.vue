<script>
export default {
  name: 'TestimonialSection',
  data(){
    return{

    }
  }

}
</script>

<template>
  <section class="debug testimonial-section">
    <p class="name-section d-flex justify-content-center align-items-start">testimonial</p>
    <div class="d-flex justify-content-end">
      <h3 class="title-section ">WHAT'S THE CUSTOMER SAY ABOUT OUR WORK</h3>
    </div>
    <div class="container-testimonial-section d-flex align-items-center justify-content-start">
      <!-- card -->
      <div class="debug testimonial-card d-flex align-items-center justify-content-center">
        <div class="debug container-testimonial-card">
          <div class="description-testimonial-card">When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .</div>
          <div class="little-container-testimonial-section">
            <div class="name-testimonial-card">Vera Duncan</div>
            <div class="company-testimonial-card">Amazon Inc.</div>
          </div>
        </div>
      </div>

      <div class="debug testimonial-card d-flex align-items-center justify-content-center">
        <div class="container-testimonial-card">
          <div class="description-testimonial-card">When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .</div>
          <div class="little-container-testimonial-section">
            <div class="name-testimonial-card">Vera Duncan</div>
            <div class="company-testimonial-card">Amazon Inc.</div>
          </div>
        </div>
      </div>

      <div class="debug testimonial-card d-flex align-items-center justify-content-center">
        <div class="container-testimonial-card">
          <div class="description-testimonial-card">When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .</div>
          <div class="little-container-testimonial-section">
            <div class="name-testimonial-card">Vera Duncan</div>
            <div class="company-testimonial-card">Amazon Inc.</div>
          </div>
        </div>
      </div>



    </div>


  </section>

</template>

<style lang="scss" scoped>
@use '../../../scss/main.scss' as *;

.testimonial-section{
  height: 980px;
  max-width: 1519px;


  .name-section{
    text-transform: uppercase;
    font-family: montserrat,Sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 19px;
    letter-spacing: 2.8px;
    // margin: 0 0 15px 23px;
    margin: 0 0 38px 23px;
    position: relative;
    &::after{
      content: "";
      height: 3px;
      margin: 13px 0 0;
      background-color: $light-green;
      position: absolute;
      // left: -71px;
      right: 1.32%;
      bottom: 6px;
      width: 50px;
    }
  }
  .title-section{
    font-family: bai jamjuree,Sans-serif;
    font-size: 45px;
    font-weight: 700;
    line-height: 49px;
    letter-spacing: -.4px;
    max-width: 678px;
    text-align: right;
    margin-right: 1.32%;
    margin-bottom: 60px;


  }

  .container-testimonial-section{
    color: $primary-color;
    // padding: 0 0 12% 11%;
    // padding: 11% 0;
    // width: 90%;
    width: calc(100% - 1.32%);
    height: 385px;
    // margin-left: 35px;
    margin-left: 1.32%;
    background-color: white;
    
    .testimonial-card{
      // width: 33.333%;
      width: calc((100% - 1.32%) / 3);
      // width: calc(100% - 1.32% / 3);
      // width: calc(100% / 3 - 1.32%);
      height: 385px;
      text-align: left;

      .container-testimonial-card{
        height: 278px;
        width: 341px;

        .description-testimonial-card{
          margin-bottom: 55px;
          color: rgba(31,30,56,.7);
          font-family: montserrat,Sans-serif;
          font-size: 16px;
          font-weight: 400;
          line-height: 25px;

        }

        .little-container-testimonial-section{

          .name-testimonial-card{
            color: $primary-color;
            font-family: bai jamjuree,Sans-serif;
            font-size: 25px;
            font-weight: 700;
            line-height: 23px;
            letter-spacing: -2px;

          }
          .company-testimonial-card{
            color: rgba(31,30,56,.5);
            font-family: montserrat,Sans-serif;
            font-size: 15px;
            font-weight: 400;
            line-height: 45px;
          }

        }

      }

    }

  }

}

</style>