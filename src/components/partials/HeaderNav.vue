<script>
import { headerLinks } from "../../data/header-nav"
export default {
  name: 'HeaderNav',
  props:{
    link: String,
    nameLink: String
  },
  data(){
    return{
      headerLinks
    }
  }

}
</script>

<template>
  <li><a :href="link">{{ nameLink }}</a></li>
</template>

<style lang="scss" scoped>
@use '../../scss/main.scss' as *;

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

</style>