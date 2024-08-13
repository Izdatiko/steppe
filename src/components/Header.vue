<script setup lang="ts">

import Logo from "@/components/Icons/LogoIcon.vue";
import SocialMedia from "@/components/SocialMedia.vue";
import Pages from "@/components/Pages.vue";
</script>

<template>
  <header class="header">
    <div class="container">
      <div class="header__wrapper">
        <div><Logo></Logo></div>
        <div class="header__wrapper-pages">
          <Pages />
        </div>
        <div class="header__wrapper-social">
          <SocialMedia />
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped lang="scss">
.header {
  width: 100%;
  background-color: $main-color;
  &__wrapper {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    width: 100%;
    padding: 19px 0;
    &-pages {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 50px;
    }
    &-social {
      display: flex;
      align-items: center;
      justify-content: flex-end;
      gap: 30px;
    }
  }
}
</style>