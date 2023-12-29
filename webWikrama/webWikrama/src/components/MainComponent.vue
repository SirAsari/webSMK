<template>
  <div class="main-container">
    <div class="main-content">
        <Hero/>
        <Section1/>
    </div>
  </div>
</template>

<script>
import Hero from './Hero.vue'
import Section1 from './sections/Section1.vue'

export default {
  name: 'MainComponent',
  components: {
    Hero,
    Section1,
  },
 
};
</script>

<style scoped>

</style>
