<script>
import { store } from "./data/store"
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import HeaderAndJumbo from './components/HeaderAndJumbo.vue'
export default {
  name: 'App',
  components:{
    HeaderAndJumbo,
    Main,
    Footer
  },
  data(){
    return{
      store
    }
  }
}
</script>

<template>
  <HeaderAndJumbo/>
  <Main/>
  <Footer/>
</template>

<style lang='scss'>
@use './scss/main.scss' as *;
@import url('https://fonts.googleapis.com/css?family=Montserrat');
@import url('https://fonts.googleapis.com/css?family=Bai+Jamjuree');

body{
  color: white;
  background-color: $primary-color;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

.debug{
    border: 1px dashed blue;
  }

  header, main, footer{
    // max-width: 1520px;
    width: 1519px;
  }

}

</style>
