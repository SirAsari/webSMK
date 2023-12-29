<template>
  <div class="container">
    <Navbar />
    <MainComponent />
  </div>
</template>

<script>
import Footer from './components/Footer.vue'
import MainComponent from './components/MainComponent.vue'
import Navbar from './components/Navbar.vue'

export default {
  name: 'App', 
  components: {
    Navbar,
    MainComponent,
    Footer,
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&family=Raleway:ital,wght@0,400;0,500;0,600;1,500;1,600&display=swap');
</style>
