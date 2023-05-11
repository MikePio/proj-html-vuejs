<script>
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  import 'swiper/css/pagination';

  // import './style.css';

  // import required modules
  import { Navigation } from 'swiper';

export default {
  name: 'ProjectSection',
  components:{
    Swiper,
    SwiperSlide,
  },
  data(){
    return{
      options: {
        slidesPerView: 3,
        loop: false,

      }
    }
  },
  setup(){
    return {
      modules: [ Navigation],
    };
  },
  methods: {


  },
  mounted() {

  }


}
</script>

<template>
  <section class="debug project-section ">
    <p class="name-section">PROJECT</p>
    <div class="container-mp d-flex justify-content-between">
      <h3 class="title-section">OUR EXPERT TRUSTED CONSULTANTS HELP CLIENTS</h3>
      <div class="container-buttons d-flex justify-content-center">
        <div class="arrow-left d-flex align-items-center justify-content-center  " ><span>&#x2190;</span></div>
        <div class="arrow-right d-flex align-items-center justify-content-center " ><span>&#x2192;</span></div>
      </div>
    </div>


    <div class="container-slider">

      <swiper
        :slidesPerView="3"
        :spaceBetween="30"
        :modules="modules"
        :navigation="false"
        class="mySwiper"
      >
        <swiper-slide><img src="public\images\DRY-1-790x592.jpg" alt="img-slider"></swiper-slide>
        <swiper-slide><img src="public\images\221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg" alt="img-slider"></swiper-slide>
        <swiper-slide><img src="public\images\z1el4c4p-790x592.jpg" alt="img-slider"></swiper-slide>

      <!-- test         -->
        <!-- <swiper-slide><img src="public\images\z1el4c4p-790x592.jpg" alt="img-slider"></swiper-slide>
        <swiper-slide><img src="public\images\z1el4c4p-790x592.jpg" alt="img-slider"></swiper-slide>
        <swiper-slide><img src="public\images\z1el4c4p-790x592.jpg" alt="img-slider"></swiper-slide>
        <swiper-slide><img src="public\images\z1el4c4p-790x592.jpg" alt="img-slider"></swiper-slide> -->
      
      </swiper>

    </div>

  </section>

</template>

<style lang="scss" scoped>
@use '../../../scss/main.scss' as *;

.project-section{
  height: 980px;

  //name section
  .name-section{
    margin: 226px 0 36px 94px;
    font-family: montserrat,Sans-serif;
    font-size: 16px;
    font-weight: 400;
    line-height: 19px;
    letter-spacing: 2px;
    position: relative;
    &::before{
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

  .container-mp{
    //title
    // margin-left: 20px;
    margin: 0 1.32%;
    .title-section{
      margin-bottom: 65px;
      // margin-left: 20px;
      // margin-left: 1.32%;

      font-family: bai jamjuree,Sans-serif;
      font-size: 45px;
      font-weight: 700;
      line-height: 49px;
      letter-spacing: -.4px;
      max-width: 829px;
    }

    .container-buttons{
      // margin-right: 1.32%;

      & div{
        // padding: 11px 12px 6px 11px;
        height: 50px;
        width: 50px;
        background-color: rgba(255,255,255,.1);
      }
    }
    .arrow-left span, .arrow-right {
      // font-size: 18px;
      // height: 20px;
    }
    .arrow-left{
      margin-right: 8px;

    }
    .arrow-right{

    }

  }


  //slider
  .container-slider{
    // margin-left: 20px;
    margin-left: 1.32%;
    height: 356px;
    max-width: 1519px;
    & img{
      // margin-right: 20px;
      margin-right: 32px;
      width: 474px;
      height: 355px;
    }

  }



}








</style>