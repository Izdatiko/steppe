<script setup lang="ts">

import Project from "@/components/Icons/Project.vue";
</script>

<template>
  <section class="home">
    <div class="home__header">
      <Project v-for="(icon, index) in 3" :key="index"/>
    </div>
    <div class="home__block">
      <img src="/img/block_1.png" alt="">
      <img src="/img/block_2.png" alt="">
    </div>
  </section>
</template>

<style scoped lang="scss">
  .home {
    display: flex;
    flex-direction: column;
    gap: 55px;
    margin: 40px 0;
    &__header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      @media (max-width: 768px) {
        justify-content: center;
        gap: 20px;
      }
    }
    &__block {
      display: flex;
      gap: 24px;
      @media (max-width: 768px) {
        flex-direction: column;
      }
      img {
        max-width: 100%;
        width: calc(50% - 12px);

        @media (max-width: 768px) {
          width: 100%;
        }
      }
    }
  }
</style>