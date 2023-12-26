<template>
    <div class="container">
      <div class="row">
        <div class="col text-center">
          <h3>Best of the best</h3>
          <p>Sebuah lembaga pendidikan yang didedikasikan untuk memaksimalkan potensi anak bangsa.</p>
        </div>
      </div>
      <div class="hero-box-container">
        <div class="hero-box hero-box-1"><p>Dipercaya oleh industri dan masyarakat</p></div>
        <div class="hero-box hero-box-2"></div>
        <div class="hero-box hero-box-3"><p>Sekolah Ramah Anak</p></div>
        <div class="hero-box hero-box-4"><p>Ekstrakulikuler Penunjang Bakat Pelajar</p></div>
        <div class="hero-box hero-box-5"><p>Melahirkan Anak Bangsa Berprestasi</p></div>
        <div class="hero-box hero-box-6"><p>Mempersiapkan Pelajar Untuk Masa Depan</p></div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Hero',
  };
  </script>
  
  <style scoped>
 .hero-box {
  display: flex;
  align-items: flex-end; 
  justify-content: flex-start; 
  padding: 10px; 
}

.hero-box p {
  font-size: 18px;
  color: white;
  font-weight: 600;
  margin: 3px; 
}

.col.text-center h3 {
  /* margin-top: px; */
  color: rgba(33, 56, 102, 1);
  font-weight: 600;
  font-size: 32px;
}

.col.text-center p {
  font-size: 18px;
  margin-left: auto; 
  margin-right: auto; 
  width: 500px;
}
.hero-box-container {
  display: grid;
  grid-template-columns: 35% 30% 5% auto;
  grid-template-rows: 186px 50px 120px;
  margin-top: 28px;
  gap: 8px;
  overflow: hidden;
}

.hero-box-1 {
  background-image: 
    linear-gradient(to top,rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)), /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-1.png);
  grid-row: 1 / 3;
  background-size: cover;
  background-position: 0px;
}

.hero-box-2 {
  background-image: 
    linear-gradient(to top,rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)), /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-2.png);
  grid-column: 2 / 4;
  background-size: cover;
  background-position: 0px -60px;
}

.hero-box-3 {
  background-image: 
    linear-gradient(to top,rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)), /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-3.png);
  background-size: cover;
  background-position: 0px -60px;
}

.hero-box-4 {
  background-image: 
    linear-gradient(to top,rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)), /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-4.png);
  grid-row: 3;
  background-size: cover;
}

.hero-box-5 {
  background-image: 
    linear-gradient(to top,rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)), /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-5.png);
  grid-row: 2 / 4;
  background-size: cover;
  background-position: 0px -20px;
}

.hero-box-6 {
  background-image: 
    linear-gradient(to top,rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)), /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-6.png);
  grid-row: 2 / 4;
  grid-column: 3 / 5;
  background-size: cover;
  background-position: 0px -39px;
}
</style>