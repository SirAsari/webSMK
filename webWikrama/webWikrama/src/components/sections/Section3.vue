<template>
    <div class="section-3-container">
    <div class="carousel-wrapper">
      <div class="carousel-bg"></div>
      <div class="carousel" @mousedown="onTouchStart" @touchstart="onTouchStart" @mousemove="onTouchMove"
        @touchmove="onTouchMove" @mouseup="onTouchEnd" @touchend="onTouchEnd" @mouseleave="onTouchEnd" ref="carousel">
        <div v-for="(slide, index) in slides" :key="index" :class="{ 'active': index === currentSlide }" class="slide"
          :style="{ transform: `translateX(-${currentSlide * 100}%)` }">
          <img :src="`/img/${slide.image}`" alt="My Image" />
        </div>
      </div>
    </div>
        <div class="flex-right-container">
            <h3>Program Keahlian</h3>
            <div class="sub-title">
                <p v-for="(text, index) in texts" :key="index" :class="[ 'text', `text${index + 1}`, { 'big': currentIndex === index } ]">
                    {{ text }}
                </p>   
            </div>
            <hr>
            <div class="description-text">
              <div class="first-row">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
                   Cras pretium magna ac tristique consectetur. Maecenas mollis 
                   consequat sodales. Vivamus quis elementum orci. 
                </p>
              </div>
              <div class="second-row">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
                   Cras pretium magna ac tristique consectetur. Maecenas mollis 
                   consequat sodales. Vivamus quis elementum orci.
                </p>
              </div>
            </div>
            <button class="left-corner-button">Baca Detail</button>
        </div>
    </div>
</template>
  
<script>
export default {
    name: 'Section3',
    data() {
        return {
            texts: ['KLN', 'HTL', 'TKJ', 'RPL', 'MMD', 'MPLB', 'PMN'], 
            currentIndex: 0, // index for the current big text
            currentSlide: 0,
            touchStartX: 0,
            touchEndX: 0,
            slides: [
                { image: 'people-kln.png' },
                { image: 'people-htl.png' },
                { image: 'people-tkj.png' },
                { image: 'people-tkj.png' },
                { image: 'people-tkj.png' },
                { image: 'people-tkj.png' },
            ],
            autoPlay: null
        };
    },
    methods: {
        showText() {
        setInterval(() => {
            this.currentIndex = (this.currentIndex + 1) % this.texts.length;
            }, 8000); // Change text every 8 seconds
        },
        nextSlide() {
    this.currentSlide = (this.currentSlide + 1) % this.slides.length;

    // Update currentIndex based on the current slide
    switch (this.currentSlide) {
      case 0:
        this.currentIndex = 0; // Corresponding index for 'KLN' slide
        break;
      case 1:
        this.currentIndex = 1; // Corresponding index for 'HTL' slide
        break;
      case 2:
        this.currentIndex = 2; // Corresponding index for 'TKJ' slides
        break;
      case 3:
        this.currentIndex = 3; // Corresponding index for 'TKJ' slides
        break;
      case 4:
        this.currentIndex = 4; // Corresponding index for 'TKJ' slides
        break;
      case 5:
        this.currentIndex = 5; // Corresponding index for 'TKJ' slides
        break;
      case 5:
        this.currentIndex = 5; // Corresponding index for 'TKJ' slides
        break;
      default:
        this.currentIndex = 6; // Corresponding index for 'PMN' slide
        break;
    }
  },
  prevSlide() {
    this.currentSlide = (this.currentSlide - 1 + this.slides.length) % this.slides.length;

    // Update currentIndex based on the current slide
    switch (this.currentSlide) {
      case 0:
        this.currentIndex = 0; // Corresponding index for 'KLN' slide
        break;
      case 1:
        this.currentIndex = 1; // Corresponding index for 'HTL' slide
        break;
      case 2:
        this.currentIndex = 2; // Corresponding index for 'TKJ' slides
        break;
      case 3:
        this.currentIndex = 3; // Corresponding index for 'TKJ' slides
        break;
      case 4:
        this.currentIndex = 4; // Corresponding index for 'TKJ' slides
        break;
      case 5:
        his.currentIndex = 5; // Corresponding index for 'TKJ' slides
        break;
      default:
        this.currentIndex = 0; // Corresponding index for 'PMN' slide
        break;
    }
  },     
        startAutoPlay() {
            this.autoPlay = setInterval(() => {
                this.nextSlide();
            }, 8000); // Slide every 8 seconds
        },
        stopAutoPlay() {
            clearInterval(this.autoPlay);
        },
        onTouchStart(e) {
            this.touchStartX = e.clientX || e.touches[0].clientX;
        },
        onTouchMove(e) {
            if (this.touchStartX === 0) return;

            const currentX = e.clientX || e.touches[0].clientX;
            const diff = this.touchStartX - currentX;

            if (Math.abs(diff) > 50) {
                if (diff > 0) {
                    this.nextSlide();
                } else {
                    this.prevSlide();
                }
                this.touchStartX = 0;
            }
        },
        onTouchEnd() {
            this.touchStartX = 0;
        }
    },
    mounted() {
        this.startAutoPlay();
        this.showText();

        // Pause autoplay on touch
        const carousel = this.$refs.carousel;
        carousel.addEventListener('touchstart', this.stopAutoPlay);
    },
    beforeDestroy() {
        clearInterval(this.autoPlay);

        const carousel = this.$refs.carousel;
        carousel.removeEventListener('touchstart', this.stopAutoPlay);
    }
};
</script>
  
<style scoped>
img {
    vertical-align: unset;
    pointer-events: none;
    user-select: none;
}
.section-3-container {
    display: flex;
    justify-content: space-around;
    margin-top: 13rem;
    margin-bottom: 10rem;
    height:fit-content;
}

.carousel-wrapper {
  position: relative;
  width: 500px; /* Set your preferred width */
  padding: 40px 20px 0 0;
}

.carousel-bg {
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 70%; /* Set the background width as needed */
  height: 100%;
  background-color: #EEF1F7; /* Set your desired background color */
  z-index: -1; /* Move the background behind the carousel */
  border-radius: 120px 120px 0px 0px;
}

.carousel {
  position: relative;
  z-index: 1; /* Ensure the images are above the background */
  overflow: hidden;
  white-space: nowrap;
  touch-action: pan-y; /* Allow vertical scroll */
}

.slide {
  text-align: center;
  display: inline-block;
  width: 100%;
  transition: transform 0.5s ease;
}

.active {
  display: inline-block;
  height: 80%;
}

.flex-right-container {
  display: flex;
  flex-direction: column;
    width: 30rem;
    margin-right: 4rem;
}

.flex-right-container h3 {
    color: rgba(33, 56, 102, 0.80);
    font-family: Poppins;
    font-weight: 600;
}

.sub-title {
  margin-top: 1.3rem;
  display: flex;
  max-height: 60px; /* Set a fixed max-height */
  flex-wrap: wrap; /* Allow the text to wrap within the fixed height */
  overflow: hidden; /* Hide overflow text beyond the fixed height */
}

.text {
  font-weight: 600;
  font-family: 'Poppins';
  margin-right: 20px; /* Adjust spacing between texts */
  transition: font-size 0.5s ease, 
  margin-top 0.5s ease; /* Apply a smooth transition */
  color: rgba(33, 56, 102, 0.588);
  margin-top: 0; /* Initially set margin-top to 0 */
  flex-shrink: 0; /* Prevent text from shrinking to fit */
  line-height: 30px; /* Set line height for the text */
  font-size: 19px;
}

.big {
  color: rgba(33, 56, 102, 0.9);
  font-size: 24px; /* Bigger font size for active text */
  font-family: Poppins;
  font-weight: 600;
  margin-top: -6px; /* Adjust the margin to shift the text upwards */
} 

hr {
    border: 2.4px solid rgba(33, 56, 102, 0.80);
     border-radius: 5px;
}

p {
    margin-bottom: 0;
}

.description-text {
  padding-top: 1rem;
}

.description-text p {
  color: rgba(33, 56, 102, 0.65);
  font-family: Poppins;
  font-size: 16px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}
.second-row p {
  margin-top: 15px;
}

.left-corner-button {
  top: 10px; 
  left: 10px;
  color: rgba(255, 255, 255, 0.8);
  border: none;
  padding: 8px 16px;
  font-size: 16px;
  cursor: pointer;
  border-radius: 5px;
  background: #80A4ED;
  box-shadow: 0px 10px 30.1px 14px rgba(128, 164, 237, 0.15);
  margin-top: auto; 
  margin-bottom: 5px;
  font-weight: 600;
  font-size: 20px;
  font-family: 'Raleway';
}

</style>
  