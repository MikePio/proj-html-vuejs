<script>
import ConsultationSection from '../components/partials/main-sections/ConsultationSection.vue'
export default {
  name: 'Main',
  components:{
    ConsultationSection
  },
  data(){
    return{

    }
  }

}
</script>

<template>
  <main>
    <ConsultationSection/>



  </main>
</template>

<style lang="scss" scoped>
@use '../scss/main.scss' as *;




</style>