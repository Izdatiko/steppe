<template>
  <div class="swiper-container">
    <swiper
        :slides-per-view="1"
        :space-between="0"
        :modules="modules"
        :pagination="true"
        :loop="true"
        class="mySwiper"
    >
      <swiper-slide v-for="(slide, index) in slides" :key="index">
          <img :src="slide" alt="slide">
      </swiper-slide>
    </swiper>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/swiper-bundle.css';
import "swiper/css/pagination";
import { Pagination } from 'swiper/modules';

const modules = [Pagination]

const slides = ref([
  '/img/photo.png',
  '/img/photo.png',
  '/img/photo.png',
  '/img/photo.png',
]);
</script>

<style scoped>
.swiper-container {
  width: 100%;
  height: 100%;
}

.swiper-slide img {
  width: 100%;
  height: auto;
  display: block;
  object-fit: cover;
}

</style>
