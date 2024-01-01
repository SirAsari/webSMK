<template>
    <div class="section-3-container">
        <div class="carousel" @mousedown="onTouchStart" @touchstart="onTouchStart" @mousemove="onTouchMove"
            @touchmove="onTouchMove" @mouseup="onTouchEnd" @touchend="onTouchEnd" @mouseleave="onTouchEnd" ref="carousel">
            <div v-for="(slide, index) in slides" :key="index" :class="{ 'active': index === currentSlide }" class="slide"
                :style="{ transform: `translateX(-${currentSlide * 100}%)` }">
                <img :src="`/img/${slide.image}`" alt="My Image" />
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    name: 'Section3',
    data() {
        return {
            currentSlide: 0,
            touchStartX: 0,
            touchEndX: 0,
            slides: [
                { image: 'people-kln.png' },
                { image: 'people-htl.png' },
                { image: 'people-tkj.png' },
            ],
            autoPlay: null
        };
    },
    methods: {
        nextSlide() {
            this.currentSlide = (this.currentSlide + 1) % this.slides.length;
        },
        prevSlide() {
            this.currentSlide = (this.currentSlide - 1 + this.slides.length) % this.slides.length;
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
}
.section-3-container {
    margin-top: 13rem;
    margin-bottom: 10rem;
    text-align: center;
    /* Center the buttons */
}

.carousel {
    border-radius: 120px 120px 0px 0px;
    background: #EEF1F7;
    width: 500px;
    /* Set your preferred width */
    overflow: hidden;
    white-space: nowrap;
    touch-action: pan-y;
    /* Allow vertical scroll */
}

.slide {
    display: inline-block;
    width: 100%;
    transition: transform 0.5s ease;
    /* background-color: blue; */
}

.active {
    display: inline-block;
}
</style>
  