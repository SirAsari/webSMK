<template>
    <div class="section-5-container">
      <div class="middle">
        <div class="section-5-text">
          <h3>Masa Depan Anda Tergantung Pada Sekolah Pilihan Anda.</h3>
          <p>
            Pilihan hari ini membentuk masa depan. Kami siap mendukung siswa
            meraih kesuksesan dengan kurikulum inspiratif dan lingkungan belajar
            yang mendukung.
          </p>
        </div>
        <img src="/img/groupOfPeople.png" alt="">
      </div>
    </div>
  </template>
  
  <style scoped>
    .section-5-container {
      background-color: #eef1f7;
      position: absolute;
      left: 0;
      right: 0;
      padding-left: 20px; 
      padding-right: 20px; 
    }
  
    .middle {
      display: flex;
      justify-content: space-between;
      padding-left: 70px; 
      padding-right: 70px; 
    }
  
    .section-5-text h3 {
      color: rgba(33, 56, 102, 0.80);
      font-family: Raleway;
      font-size: 38px;
      font-style: normal;
      font-weight: 600;
      line-height: normal;
      letter-spacing: 0.608px;
      padding-top: 68px;
    }
  
    .section-5-text p {
      color: rgba(33, 56, 102, 0.65);
      font-family: Raleway;
      font-size: 18px;
      font-style: normal;
      font-weight: 500;
      line-height: 134.466%;
      letter-spacing: 0.306px;
      padding-top: 16px;
      width: 555px;
    }
  
    /* Media query for responsiveness */
    @media screen and (max-width: 768px) {
      .middle {
        padding-left: 5px; /* Adjust the padding-left value for smaller screens */
        padding-right: 5px; /* Adjust the padding-right value for smaller screens */
      }
    }
  </style>
  