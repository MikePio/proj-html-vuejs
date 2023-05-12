<script>
export default {
  name: 'BlogSection',
  data(){
    return{

    }
  }

}
</script>

<template>
  <section class="debug blog-section ">
  <p class="name-section">BLOG</p>
  <div class="container-title-blog-section d-flex align-items-center justify-content-between">
    <h3 class="title-section">THE RECENT NEWS YOU MUST READ IT</h3>
    <button>VIEW ALL</button>
  </div>
  <div class="big-container-cards-blog d-flex justify-content-between">
    <!-- cards -->
    <div class="card-blog">
      <img src="public/images/startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg" alt="img-card">
      <div class="container-card-blog d-flex justify-content-center align-items-center">
        <div class="little-container-card-blog d-flex flex-column justify-content-around align-items-start">
          <div class="d-flex ">
            <div class="date">july 4, 2019</div>
            <div class="name-user mx-4">by paul</div>
          </div>
          <div class="title-container-card-blog">Canadian Consulting Firm <br>acquired by UK Giant</div>
          <div class="description-container-card-blog">When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but </div>
        </div>
      </div>
    </div>

    <div class="card-blog">
      <img src="public/images/business-people-working-together-on-project-and-5FHSKBL-1390.jpg" alt="img-card">
      <div class="container-card-blog d-flex justify-content-center align-items-center">
        <div class="little-container-card-blog d-flex flex-column justify-content-around align-items-start">
          <div class="d-flex ">
            <div class="date">july 4, 2019</div>
            <div class="name-user mx-4">by paul</div>
          </div>
          <div class="title-container-card-blog">Canadian Consulting Firm <br>acquired by UK Giant</div>
          <div class="description-container-card-blog">When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but </div>
        </div>
      </div>
    </div>
  </div>

  </section>

</template>

<style lang="scss" scoped>
@use '../../../scss/main.scss' as *;

.blog-section{
  // height: 1090px;
  margin-bottom: 337px;
  h3.title-section{
    font-family: bai jamjuree,Sans-serif;
    font-size: 45px;
    font-weight: 700;
    line-height: 49px;
    letter-spacing: -.4px;
    max-width: 1089px;
  }
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
  .container-title-blog-section{
    width: calc(100% - 1.32%);
    margin: 0 1.32% 60px;
    button{
      margin: 0 1.32%;
      font-family: montserrat,Sans-serif;
      text-transform: uppercase;
      border: none;
      width: 227px;
      height: 64px;
      background-color: $light-green;
      text-shadow: 0 0 10px transparent;
        &:hover{
          background-color: $secondary-color;
          color: #fff;
        }
    }
    
  }

  .big-container-cards-blog{
    width: calc(100% - 1.32% - 1.32%);
    margin: 0 1.32%;

    .card-blog{
      position: relative;
      img{
        width: 726px;
        height: 544px;
      }
      
      .container-card-blog{
        width: 581px;
        height: 320px;
        background-color: #fff;
        position: absolute;
        right: 0;
        bottom: -100px;
        z-index: 2;
        text-align: left;
        &:hover{
          background-color: $light-green;
          
        }
        .little-container-card-blog{
          height: 215px;
        }
        .date, .name-user{
          font-family: montserrat,Sans-serif;
          font-size: 16px;
          font-weight: 500;
          text-transform: lowercase;
          line-height: 20px;
          color: #f81d39;
        }
        .title-container-card-blog{
          color: #000;
          font-family: bai jamjuree,Sans-serif;
          font-size: 30px;
          font-weight: 500;
          line-height: 30px;
          letter-spacing: -2px;
        }
        .description-container-card-blog{
          color: rgba(31,30,56,.6);
          font-family: montserrat,Sans-serif;
          font-size: 16px;
          font-weight: 400;
          line-height: 25px;
          width: 384px;
          height: 77px;
        }

      }
    }
  }
}
</style>