<script>
// import { headerLinks } from "../../data/header-nav"
import { headerLinks } from "../data/header-nav"
import HeaderNav from './partials/HeaderNav.vue'
export default {
  name: 'Header',
  components:{
    HeaderNav
  },
  data(){
    return{
      headerLinks
    }
  }

}
</script>

<template>
  <!-- <header class="debug d-flex col align-items-center justify-content-center"> -->
  <header class="debug d-flex col align-items-start  justify-content-center">
    <div class=" container-header w-100 d-flex justify-content-between align-items-center">
      <!-- logo -->
      <div class=" row-logo row align-items-center">
          <!-- <img class="logo" src="public\images\logotype.png" alt="logo">   -->
          <img class=" logo" src="public\images\logotype-2-300x50.png" alt="logo">  
      </div>
      <!-- nav-list -->
      <div class=" row justify-content-end">
        <ul class="nav-list d-flex ">
        <!-- //* lista statica -->
          <!-- <li>Home</li>
          <li>About</li>
          <li>Projects</li>
          <li>Services</li>
          <li>Blog</li>
          <li>Contact</li> -->
          <!-- //*lista dinamica -->
          <!-- <li v-for="(headerLink, index) in headerLinks" :key="index" >{{ headerLink.name }}</li> -->
          <!-- <li v-for="(headerLink, index) in headerLinks" :key="index"><a :href="`${headerLink.url}`">{{ headerLink.name }}</a></li> -->
          <!-- //*lista dinamica CON LE PROPS-->
          <HeaderNav
            v-for="(headerLink, index) in headerLinks" 
            :key="index"
            :link="headerLink.url"
            :nameLink=" headerLink.name" 
            />
          <!-- <li><a :href="link">{{ nameLink }}</a></li> -->
        </ul>
      </div>

    </div>
  </header>

</template>

<style lang="scss" scoped>
@use '../scss/main.scss' as *;



header{
  // height: 296px;
  // height: 82px;
  // width: 100%;


  .container-header{
    padding: 0px 33px;
  }
  .row-logo{
    // padding-top: 15px;
    padding-bottom: 30px;
    // padding: 15px 0;
    img{
      // width: 120px;
      height: 19px;
      filter: invert(32%) sepia(95%) saturate(6840%) hue-rotate(345deg) brightness(109%) contrast(95%);
      cursor: pointer;
    }
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
      // height: 120px;
      height: 82px;
      margin: 0 20px;
      font-size: 15px;
      font-weight: 200;
      font-family: 'Montserrat', sans-serif;
      position: relative;
      &:hover{
        cursor: pointer;
      }
      &::after{
        content: "";
        position: absolute;
        left: 0;
        top: 0;
        width: 0;
        transition: width 0.3s ease-out, left 0.3s ease-out;
        height: 3px;
        background-color: #ffffff;
      }
      &:hover::after{
        width: 100%;
        left: 0;
      }
      &:first-child{
        font-weight: 600;
      }
      &:first-child::after{
        content: "";
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 3px;
        background-color: #ffffff;
        //OPPURE
        // content: "";
        // position: absolute;
        // left: 0;
        // top: 0;
        // width: 0;
        // border-top: 6px solid #ffffff;
        // width: 100%;
      }

    }
    a{
      text-decoration: none;
      color: #ffffff;
    }

  }
}

</style>