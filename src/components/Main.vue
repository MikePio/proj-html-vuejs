<script>
import ConsultationSection from '../components/partials/main-sections/ConsultationSection.vue'
import AboutUsSection from '../components/partials/main-sections/AboutUsSection.vue'

export default {
  name: 'Main',
  components:{
    ConsultationSection,
    AboutUsSection
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
    <AboutUsSection/>



  </main>
</template>

<style lang="scss" scoped>
@use '../scss/main.scss' as *;




</style>