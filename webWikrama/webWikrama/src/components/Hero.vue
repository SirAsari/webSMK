<template>
    <div class="container">
      <div class="row">
        <div class="col text-center">
          <h3>Best Of The Best</h3>
          <p>Sebuah lembaga pendidikan yang didedikasikan untuk memaksimalkan potensi anak bangsa.</p>
        </div>
      </div>
    </div>
    <div class="hero-content">
      <div class="hero-box hero-box-1">1</div>
      <div class="hero-box hero-box-2">2</div>
      <div class="hero-box hero-box-3">3</div>
      <div class="hero-box hero-box-4">4</div>
      <div class="hero-box hero-box-5">5</div>
      <div class="hero-box hero-box-6">6</div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Hero',
  };
  </script>
  
  <style scoped>
.hero-content {
  position: relative;
  width: 600px; /* Adjust the width of the container */
  height: 600px; /* Adjust the height of the container */
}

.hero-box {
  position: absolute;
  font-size: 40px;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* Custom styles for each box */
.hero-box-1 {
  background-color: #70e9c9;
  width: 300px;
  height: 200px;
  top: 0;
  left: 0;
}

.hero-box-2 {
  background-color: #63dbbb;
  width: 200px;
  height: 400px;
  top: 0;
  right: 0;
}

.hero-box-3 {
  background-color: #51c9a9;
  width: 200px;
  height: 200px;
  top: 200px;
  left: 0;
}

.hero-box-4 {
  background-color: #3dafa0;
  width: 100px;
  height: 100px;
  top: 400px;
  left: 200px;
}

.hero-box-5 {
  background-color: #309d96;
  width: 100px;
  height: 100px;
  top: 400px;
  left: 300px;
}

.hero-box-6 {
  background-color: #1e897a;
  width: 200px;
  height: 100px;
  top: 500px;
  left: 0;
}
</style>