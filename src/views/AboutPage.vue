<script setup lang="ts">

import Swiper from "@/components/Swiper.vue";
</script>

<template>
  <section class="about">
  <swiper />
    <div class="about__info">
      <div class="about__header">
        <h1>О нас</h1>
        <div class="about__line"/>
      </div>
      <div class="about__text">
        <h2>«Donec nulla erat, laoreet sit amet sodales a, lobortis vitae dui.»</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse ullamcorper sem quis massa aliquet,
          vel accumsan neque facilisis. Aliquam eget odio auctor, laoreet justo sed, interdum justo.
          Donec posuere vestibulum euismod. Sed finibus arcu vel rutrum dictum. In nec luctus metus,
          condimentum malesuada ex. Nam faucibus mauris nunc, sit amet condimentum ante accumsan a. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse ullamcorper sem quis massa aliquet,
          vel accumsan neque facilisis. Aliquam eget odio auctor, laoreet justo sed, interdum justo.
          Donec posuere vestibulum euismod. Sed finibus arcu vel rutrum dictum. In nec luctus metus,
          condimentum malesuada ex. Nam faucibus mauris nunc, sit amet condimentum ante accumsan a. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse ullamcorper sem quis massa aliquet,
          vel accumsan neque facilisis. Aliquam eget odio auctor, laoreet justo sed, interdum justo.
          Donec posuere vestibulum euismod. Sed finibus arcu vel rutrum dictum. In nec luctus metus,
          condimentum malesuada ex. Nam faucibus mauris nunc, sit amet condimentum ante accumsan a.</p>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
.about {
  display: flex;
  flex-direction: column;
  gap: 40px;
  margin-bottom: 80px;
  &__info {
    display: flex;
    flex-direction: column;
    gap: 60px;
  }
  &__header {
    display: flex;
    align-items: center;
    gap: 50px;
    h1 {
      color: $main-color;
      font-size: 36px;
      font-weight: 700;
      line-height: 43.52px;
      letter-spacing: 0.5em;
      text-align: left;
      white-space: nowrap;
      text-transform: uppercase;
    }
  }
  &__line {
    width: 100%;
    height: 1px;
    background-color: $main-color;
  }
  &__text {
    display: flex;
    flex-direction: column;
    gap: 20px;
    h2 {
      color: $main-color;
      font-size: 36px;
      font-weight: 700;
      line-height: 43.52px;
      text-align: left;
    }
    p {
      color: $main-color;
      font-size: 18px;
      font-weight: 400;
      line-height: 21.6px;
      text-align: left;
    }
  }
}
</style>