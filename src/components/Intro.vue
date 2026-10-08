<template>
  <div class="mainPage">

    <div class="intro">
      <div class="logo en">
          <span class="p">P</span>
          <span class="a">A</span>
          <span class="n">N</span>
          <span class="d">D</span>
          <span class="a2">A</span>
          <span class="dash">-</span>
          <span class="a3">A</span>
          <span class="i">i</span>
      </div>

      <p class="description kr">
        판다 AI의 대화형 제작 시스템을 통해 쉽고 빠르게<br />
        제품 페이지와 마케팅 콘텐츠를 제작해 보세요.
      </p>

      <button class="startBtn kr">
        바로 시작하기
      </button>
    </div>


    <div class="swiperArea">
      <Swiper
        :modules="modules"
        :slides-per-view="4.5"
        :space-between="16"
        :loop="true"
        :speed="2000"
        :autoplay="{
          delay: 0,
          disableOnInteraction: false
        }"
        :allow-touch-move="false"
        @swiper="onSwiper"
      >
        <SwiperSlide
          v-for="(image, index) in images"
          :key="index"
        >
          <img :src="image" alt="" />
        </SwiperSlide>
      </Swiper>
    </div>

  </div>
</template>

<script>
import { Swiper, SwiperSlide } from 'swiper/vue'
import { Autoplay } from 'swiper/modules'

console.log('Autoplay:', Autoplay)

import 'swiper/css'

import swiperImg1 from '../images/home_swiper1.jpg'
import swiperImg2 from '../images/home_swiper2.jpg'
import swiperImg3 from '../images/home_swiper1.jpg'
import swiperImg4 from '../images/home_swiper2.jpg'
import swiperImg5 from '../images/home_swiper1.jpg'
import swiperImg6 from '../images/home_swiper2.jpg'

export default {
  name: 'MainPage',

  components: {
    Swiper,
    SwiperSlide
  },

  data() {
    return {
      modules: [Autoplay],

      images: [
        swiperImg1,
        swiperImg2,
        swiperImg3,
        swiperImg4,
        swiperImg5,
        swiperImg6,

        swiperImg1,
        swiperImg2,
        swiperImg3,
        swiperImg4,
        swiperImg5,
        swiperImg6
      ]
    }
  }
}
</script>

<style scoped>
.mainPage {
  position: relative;
  width: 100%;
  background: linear-gradient(
    to bottom,
    #F2F2F2 0%,
    #F2F2F2 85%,
    #F7F7F7 92%,
    #FCFCFC 97%,
    #FFFFFF 100%
  );
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 100px;
  height: 100vh;
}

.intro {
  width: 100%;
  display: flex;
  flex-direction: column;
  gap: 50px;
  text-align: center;
  align-items: center;
  justify-content: center;
}

.logo {
  display: inline-flex;
  align-items: center;
  font-size: 80px;
  font-weight: 800;
  line-height: 1;
  letter-spacing: 1.2;
}

/* P */
.logo .p {
  color: #E3B9FF;
}

/* A */
.logo .a {
  color: #B7CFFF;
}

/* N */
.logo .n {
  color: #83CFFF;
}

/* D */
.logo .d {
  color: #B4D5E8;
}

/* A */
.logo .a2 {
  color: #F3B7B7;
}

/* - */
.logo .dash {
  color: #F4B1B1;
  margin: 0 2px;
}

/* A */
.logo .a3 {
  color: #FFBE8A;
}

/* i */
.logo .i {
  color: #FFB26D;
}


.description {
  font-size: 30px;
  font-weight: 600;
  color: #111;
}

.startBtn {
  border: none;
  padding: 1rem 3rem;
  border-radius: 40px;
  background: #999;
  color: #fff;
  font-size: 32px;
  cursor: pointer;
  transition: 0.2s;
}

.startBtn:hover {
  background: #83CFFF;
}

.swiperArea {
  width: 100%;
  overflow: hidden;
}

.swiperArea :deep(.swiper) {
  width: 100%;
  height: 100%;
}

.swiperArea :deep(.swiper-wrapper) {
  transition-timing-function: linear !important;
}

.swiperArea :deep(.swiper-slide) {
  height: 600px;
}

.swiperArea :deep(.swiper-slide img) {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>