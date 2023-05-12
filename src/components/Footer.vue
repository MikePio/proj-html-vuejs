<script>
export default {
  name: 'Footer',
  data(){
    return{

    }
  }

}
</script>

<template>
  <footer>
    <div class="container-footer">

      <div class="nav-row d-flex justify-content-between">
          <img class="logo-footer" src="public/images/logotype-2-300x50.png" alt="logo-footer">
        <nav>
          <ul class="nav-list d-flex ">
            <li>Home</li>
            <li>About</li>
            <li>Projects</li>
            <li>Services</li>
            <li>Blog</li>
            <li>Contact</li>
          </ul>
        </nav>
        <div class="empty-div"></div>
      </div>

      <div class="terms-of-use d-flex justify-content-between align-items-center">
        <div class="col-mp">
          <h6>Terms of use</h6>
          <h3>Privacy Environmental Policy</h3>
        </div>
        <div class="col-mp">
          <div>Copyright © 2023 Phlox Consulting. All Rights Reserved.</div>
        </div>
      </div>

    </div>
  </footer>

</template>

<style lang="scss" scoped>
@use '../scss/main.scss' as *;

footer{
  // height: 305px;
  // height: 188px;
  margin-bottom: 40px;
  .container-footer{
    margin: 0 2.30%;
    position: relative;
    .nav-row{
      width: calc(100% - 2.30% - 2.30%);

    }

    .logo-footer{
      height: 24px;
      width: 140px;
      justify-self: start !important;
    }
    nav{
      justify-self: center !important;

    }
    .nav-list {
      // reset liste
      ul {
        list-style-type: none;
      }
      & li {
        list-style: none;
        text-transform: uppercase;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin-right: 26px;
        font-size: 15px;
        font-family: 'Montserrat', sans-serif;
        color: #aaa;
        font-weight: 400;
        &:hover{
          cursor: pointer;
          color: $secondary-color;
        }
      }
    }
  }

  .terms-of-use{
    border-top: 0.5px solid rgba(255,255,255,.4);
    color: rgba(255,255,255,.4);

    padding-top: 40px;
    margin-top: 80px;

    h6{
      font-family: montserrat,Sans-serif;
      margin: 0 0 15px;
      font-size: 14px;
      font-weight: 400;
    }
    h3{
      font-family: montserrat,Sans-serif;
      line-height: 1.5em;
      font-size: 14px;
      font-weight: 400;
    }

    div{
      font-family: montserrat,Sans-serif;
      text-transform: capitalize;
      line-height: 1.2em;
      font-size: 14px;
      font-weight: 400;
    }

  }










}

</style>