<template>
  <div class="section-4-slider">
    <div class="slide-track">
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>

      <!-- another slide -->
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
      <div class="slide">
        <div class="slide-content"></div>
      </div>
    </div>
  </div>
</template>
  
<script>

</script>
  
<style scoped>
.section-4-slider {
  height: 250px;
  margin: auto;
  position: relative;
  width: 90%;
  display: grid;
  place-items: center;
  overflow: hidden;
}
.slide-track {
  display: flex;
  width: calc(250px * 18);
  animation: scroll 40s linear infinite;
}
@keyframes scroll {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(calc(-250px * 9));
  }
}

.slide {
  height: 200px;
  width: 250px;
  display: flex;
  align-items: center;
  padding: 15px;
}
.slide-content {
  width: 100%;
  height: 100%;
  background-color: blue;
}

</style>
