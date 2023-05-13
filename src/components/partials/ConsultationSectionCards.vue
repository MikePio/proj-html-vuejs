<script>
import { consultationCards } from "../../data/consultation-cards"
// import { consultationCards } from "../../../data/consultation-cards"

export default {
  name: 'ConsultationSectionCards',
  props:{
    imagePath: String,
    title: String,
    description: String
  },
  data(){
    return{
      consultationCards
    }
  }

}
</script>

<template>

  <div class="card-mp d-flex justify-content-center">
  <div class="container-img-card d-flex align-items-center justify-content-center">
    <img class="img-card" :src="imagePath" alt="img-card">
  </div>
  <div class="description-card">
    <h3>{{ title }}</h3>
    <p>{{ description }}</p>
  </div>
</div> 

</template>

<style lang="scss" scoped>
@use '../../scss/main.scss' as *;

.card-mp{
      margin-bottom: 130px;

      .container-img-card{
        background-color: $secondary-color;
        // border-radius: 50%;
        border-radius: 50px;
        height: 65px;
        width: 65px;
        margin-right: 50px;

        img{
          width: 34px;
        }
      }
    }

  h6, h3{
    font-family: bai jamjuree,Sans-serif;

  }
  h6{
    font-size: 30px;
    font-weight: 700;
    line-height: 40px;
    letter-spacing: -1px;
    position: relative;
    margin: 124px 0 123px;
    text-transform: uppercase;

    &::after{
      content: "";
      height: 3px;
      width: 810px;
      width: 788px;
      margin: 0 0 0 43px;
      background-color: $light-green;

      position: absolute;
      top: 50%;
      // left: 0;
    }
  }
  .description-card{
    width: 330px;
    margin-right: 200px;

    h3{
        font-size: 25px;
      font-weight: 700;
      line-height: 33px;
      letter-spacing: -1px;
      text-transform: uppercase;
      padding: 13px 0 0;
    }
    p{
      font-family: montserrat,Sans-serif;
      font-size: 16px;
      font-weight: 400;
      line-height: 25px;

    }
  }


</style>