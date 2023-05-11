<script>
import ConsultationSection from '../components/partials/main-sections/ConsultationSection.vue'
import AboutUsSection from '../components/partials/main-sections/AboutUsSection.vue'
import ProjectSection from '../components/partials/main-sections/ProjectSection.vue'
import TestimonialSection from '../components/partials/main-sections/TestimonialSection.vue'
import BlogSection from '../components/partials/main-sections/BlogSection.vue'
import AboutWorkSection from '../components/partials/main-sections/AboutWorkSection.vue'


export default {
  name: 'Main',
  components:{
    ConsultationSection,
    AboutUsSection,
    ProjectSection,
    TestimonialSection,
    BlogSection,
    AboutWorkSection
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
    <ProjectSection/>
    <TestimonialSection/>
    <BlogSection/>
    <AboutWorkSection/>



  </main>
</template>

<style lang="scss" scoped>
@use '../scss/main.scss' as *;




</style>