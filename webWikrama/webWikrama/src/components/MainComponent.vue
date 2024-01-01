<template>
  <div class="main-container">
    <div class="main-content">
        <Hero/>
        <Section1/>
        <Services/>
        <Section3/>
    </div>
  </div>
</template>

<script>
import Hero from './Hero.vue'
import Section1 from './sections/Section1.vue'
import Services from './sections/Services.vue'
import Section3 from './sections/Section3.vue'

export default {
  name: 'MainComponent',
  components: {
    Hero,
    Section1,
    Services,
    Section3, 
  },
 
};
</script>

<style scoped>

</style>
