<template>
  <div class="service-container">
    <div class="service-title">
      <h3>Layanan Kami</h3>
    </div>
    <div class="card-container">
      <div class="service-card">
        <img src="/img/headBookIcon.png" alt="service-card 1 icon">
        <h3>Beragam Bidang Keahlian</h3>
        <p>Kami Menyediakan Pembelajaran dengan berbagai macam bidang keahlian: RPL, MMD, TKJ, TBG, PMN, MPLB</p>
      </div>
      <div class="service-card">
        <img src="/img/peopleUpArrowIcon.png" alt="service-card 2 icon">
        <h3>Lingkungan Pembelajaran Optimal</h3>
        <p>Kami menyediakan lingkungan belajar unggul yang mendukung pertumbuhan dan perkembangan siswa.</p>
      </div>
      <div class="service-card">
        <img src="/img/smilerIcon.png" alt="service-card 3 icon">
        <h3>Prestasi di Tingkat Internasional</h3>
        <p>SMK Wikrama Bogor telah mendapat penghargaan global, mengukuhkan reputasi kami dalam memberikan pendidikan berkualitas.</p>
      </div>
      <div class="service-card">
        <img src="/img/penToolIcon.png" alt="service-card 4 icon">
        <h3>Pembelajaran Berstandar Nasional</h3>
        <p>Tuntunan berkualitas dari pendidik terbaik, membantu siswa meraih kemajuan belajar yang terbaik.</p>
      </div>
      <div class="service-card">
        <img src="/img/handLoveIcon.png" alt="service-card 5 icon">
        <h3>Masih Banyak Lagi</h3>
        <p>Tertarik untuk melihat apa lagi yang kami tawarkan? </p>
        <button class="service-button">Klik disini</button>
      </div>
    </div>
  </div>
</template>

<style scoped>
.service-container {
  padding-top: 40rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.service-title h3 {
  font-size: 2rem;
  font-weight: 600;
  font-family: 'Poppins', sans-serif;
  color: #213866;
  margin-bottom: 3rem;
  text-align: center;
}

.card-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 3rem; 
  margin: 0 auto;
  max-width: 1100px; 
}

.service-card {
  text-align: center;
  border-radius: 12px;
  background: #FFF;
  box-shadow: 0px 8px 48.4px 3px rgba(45, 146, 140, 0.13);
  width: 316px;
    padding: 24px 36px;
}

.service-card img {
  width: 65px;
  height: 69px;
}

.service-card h3 {
  margin-top: 26px;
  font-size: 1.2rem;
  color: rgba(33, 56, 102, 0.79);
  font-weight: 600;
  font-style: italic;
  font-family: 'Raleway', sans-serif;
  margin-bottom: 1rem;
}

.service-card p {
  color: rgba(33, 56, 102, 0.80);
  font-size: 1rem;
  line-height: 1.5;
}

.service-button {
  padding: 0.5rem 1rem;
  border: none;
  border-radius: 6px;
  background-color: #3a8bcd;
  color: white;
  font-size: 1rem;
  cursor: pointer;
  transition: background-color 0.3s ease;
  margin-top: 15px;
}

.service-button:hover {
  background-color: #1f5f87;
}
</style>
