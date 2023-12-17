<template>
  <div class="main-container">
    <div class="main-content">
        <Hero/>
    </div>
  </div>
</template>

<script>
import Hero from './Hero.vue'

export default {
  name: 'MainComponent',
  components: {
    Hero,
  },
 
};
</script>

<style scoped>

</style>
