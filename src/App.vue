<template>
  <Header/>
  <Section1/>
  <Section2/>
  <Section3/>
  <Testimonials/>
  <ShowImg/>
  <Footer/>
</template>

<script>
import Header from './components/Header.vue'
import Section1 from './components/Section1.vue'
import Section2 from './components/Section2.vue'
import Section3 from './components/Section3.vue'
import Testimonials from './components/Testimonials.vue'
import ShowImg from './components/ShowImg.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Section1,
    Section2,
    Section3,
    Testimonials,
    ShowImg,
    Footer
  }
}
</script>

<style>

</style>
