<script>
import { socialIcons } from "../../data/social-icons"
export default {
  name: 'FooterSocialIcons',
  props:{
    linkSocial: String,
    nameIcon: String
  },
  data(){
    return{
      socialIcons
    }
  }

}
</script>

<template>
  <li><a :href="linkSocial"><i :class="nameIcon"></i></a></li>
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
        margin-right: 26px;
        font-size: 15px;
        font-family: 'Montserrat', sans-serif;
        color: #aaa;
        font-weight: 400;
        &:last-child{
          margin-right: 0;
        }
        &:hover{
          cursor: pointer;
          color: $secondary-color;
        }
      }

    }
    .social-icons li i{
      color: #fff;
      font-size: 20px;

      &:hover{
        cursor: pointer;
        color: $secondary-color;
      }
    }
    a{
      text-decoration: none;
      color: #fff;
      // color: #ffffff;
      &:hover{
        cursor: pointer;
        color: $secondary-color;
      }
    }

</style>