<script>
export default {
  name: 'AboutWorkSection',
  data(){
    return{

    }
  }

}
</script>

<template>
  <section class="debug about-work-section d-flex align-items-center justify-content-center">
    <div class="container-about-work-section d-flex flex-column align-items-center justify-content-around">
      <h6>LET'S TALK ABOUT WORK</h6>
      <p>A wonderful serenity has taken possession Far far away, behind the word mountains.</p>
      <button>GET STARTED</button>
    </div>

  </section>

</template>

<style lang="scss" scoped>
@use '../../../scss/main.scss' as *;

.about-work-section{
  height: 460px;
  background-image: url('public/images/business-people-working-together-on-project-and-B3MZ4TX.jpg');
  background-position: center;
  margin-bottom: 80px;
  .container-about-work-section{
    width: 100%;
    height: 228px;
    h6{
      font-family: bai jamjuree,Sans-serif;
      font-size: 45px;
      font-weight: 700;
      line-height: 60px;
      letter-spacing: -.5px;
      margin: 0;
      text-align: center;
    }
    p{
      font-family: montserrat,Sans-serif;
      font-size: 16px;
      font-weight: 400;
      line-height: 25px;
      color: rgba(255,255,255,.8);
      max-width: 444px;
      text-align: center;
    }
    button{
      font-family: montserrat,Sans-serif;
      text-transform: uppercase;
      border: none;
      // padding: 23px 57px;
      width: 227px;
      height: 64px;
      background-color: $primary-color;
      color: #fff;
      text-shadow: 0 0 10px transparent;
        &:hover{
          background-color: $light-green;
          color: $primary-color;
        }
    }




  }



}

</style>