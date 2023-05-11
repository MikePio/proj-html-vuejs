<script>
export default {
  name: 'ConsultationSection',
  data(){
    return{

    }
  }

}
</script>

<template>
  <section class="debug consultation-section d-flex justify-content-end">
    <div class="container-consultation-section">
      <h6>Our consultants can help you</h6>
      <div class="container-cards d-flex flex-wrap">
        <div class="card-mp d-flex justify-content-center">
          <div class="container-img-card d-flex align-items-center justify-content-center">
            <img class="img-card" src="public/img-extra/line-graph.svg" alt="img-card">
          </div>
          <div class="description-card">
            <h3>STATISTICAL CONSULTING</h3>
            <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
          </div>
        </div>
        <div class="card-mp d-flex justify-content-center">
          <div class="container-img-card d-flex align-items-center justify-content-center">
            <img class="img-card" src="public/img-extra/shout.svg" alt="img-card">
          </div>
          <div class="description-card">
            <h3>DIGITAL CONSULTING</h3>
            <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
          </div>
        </div>
        <div class="card-mp d-flex justify-content-center">
          <div class="container-img-card d-flex align-items-center justify-content-center">
            <img class="img-card" src="public\img-extra\Path-13.svg" alt="img-card">
          </div>
          <div class="description-card">
            <h3>BANKING CONSULTING</h3>
            <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
          </div>
        </div>
        <div class="card-mp d-flex justify-content-center">
          <div class="container-img-card d-flex align-items-center justify-content-center">
            <img class="img-card" src="public\img-extra\target.svg" alt="img-card">
          </div>
          <div class="description-card">
            <h3>ENTERPRISE CONSULTING</h3>
            <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a</p>
          </div>
        </div>
      </div>

    </div>
  </section>

</template>

<style lang="scss" scoped>
@use '../../../scss/main.scss' as *;

.consultation-section{
  // min-height: 895px;
  height: 895px;
  color: $primary-color;

  .container-consultation-section{
    padding: 0 0 12% 11%;
    // width: 90%;
    width: 100%;
    // margin-left: 35px;
    margin-left: 2.30%;
    background-color: white;

  }
  .container-cards{
    // padding: 0 0 12% 11%;
    width: 100%;

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

}

</style>