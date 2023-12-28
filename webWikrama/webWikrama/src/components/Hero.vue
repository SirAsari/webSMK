<template>
  <div class="container">
    <div class="row">
      <div class="col text-center">
        <h3>Best of the best</h3>
        <p>Sebuah lembaga pendidikan yang didedikasikan untuk memaksimalkan potensi anak bangsa.</p>
      </div>
    </div>
    <div class="hero-box-container">
      <img src="/img/headerIcons-left.png" alt="left icon" class="left-header-icon">
      <div class="hero-box hero-box-1">
        <p>Dipercaya oleh industri dan masyarakat</p>
      </div>
      <div class="hero-box hero-box-2">
        <p>Menghasilkan lulusan yang diminati Industri</p>
      </div>
      <div class="hero-box hero-box-3">
        <p>Sekolah Ramah Anak</p>
      </div>
      <div class="hero-box hero-box-4">
        <p>Ekstrakulikuler Penunjang Bakat Pelajar</p>
      </div>
      <div class="hero-box hero-box-5">
        <p>Melahirkan Anak Bangsa Berprestasi</p>
      </div>
      <div class="hero-box hero-box-6">
        <p>Mempersiapkan Pelajar Untuk Masa Depan</p>
      </div>
      <img src="/img/headerIcons-right.png" alt="right icon" class="right-header-icon">
    </div>
    <div class="button-container">
      <button class="primary-button">Daftar Sekarang</button>
      <button class="secondary-button">Konsultasi</button>
    </div>
  </div>
</template>
  
<script>
export default {
  name: 'Hero',
};
</script>
  
<style scoped>
.button-container {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 26px;
}

.primary-button {
  background-color: #2D928C;
  color: white;
  font-weight: 600;
  font-size: 19px;
  padding: 8px 16px;
  border: none;
  border-radius: 6px;
  box-shadow: 0px 10px 24px 0px rgba(45, 146, 140, 0.25);

}

.secondary-button {
  margin-left: 16px;
  background-color: #D7DFDF;
  color: #62646B;
  font-weight: 600;
  font-size: 19px;
  padding: 8px 16px;
  border: none;
  border-radius: 6px;
  padding: 8px 36px;
}

.right-header-icon {
  position: absolute;
  width: 155px;
  opacity: 0.9;
  top: -70px;
  right: -70px;
}

.left-header-icon {
  left: -86px;
  top: -79px;
  position: absolute;
  width: 155px;
  opacity: 0.9;
}

.hero-box p {
  width: 250px;
}

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
  position: relative;
  display: grid;
  grid-template-columns: 35% 30% 5% auto;
  grid-template-rows: 186px 50px 120px;
  margin-top: 24px;
  gap: 8px;
  box-shadow:
  1.1px 4.6px 5.3px rgba(0, 0, 0, 0.016),
  3.6px 15.4px 17.9px rgba(0, 0, 0, 0.024),
  16px 69px 80px rgba(0, 0, 0, 0.04)
;
}

.hero-box-1 {
  background-image:
    linear-gradient(to top, rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)),
    /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-1.png);
  grid-row: 1 / 3;
  background-size: cover;
  background-position: 0px;
  border-radius: 12px 0 0 0;
}

.hero-box-2 {
  background-image:
    linear-gradient(to top, rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)),
    /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-2.png);
  grid-column: 2 / 4;
  background-size: cover;
}

.hero-box-3 {
  background-image:
    linear-gradient(to top, rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)),
    /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-3.png);
  background-size: cover;
  border-radius: 0 12px 0 0;
}

.hero-box-4 {
  background-image:
    linear-gradient(to top, rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)),
    /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-4.png);
  grid-row: 3;
  background-size: cover;
  border-radius: 0 0 0 12px;
}

.hero-box-5 {
  background-image:
    linear-gradient(to top, rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)),
    /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-5.png);
  grid-row: 2 / 4;
  background-size: cover;
  background-position: 0px -20px;
}

.hero-box-6 {
  background-image:
    linear-gradient(to top, rgba(68, 78, 97, 0.60), rgba(86, 98, 121, 0.40), rgba(145, 153, 168, 0.20), rgba(217, 217, 217, 0)),
    /* Gradient layer - starts dark from bottom to transparent */
    url(../img/headerCard-6.png);
  grid-row: 2 / 4;
  grid-column: 3 / 5;
  background-size: cover;
  border-radius: 0 0 12px 0;
}</style>