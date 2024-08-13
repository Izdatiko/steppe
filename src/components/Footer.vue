<script setup lang="ts">

import Logo from "@/components/Icons/LogoIcon.vue";
import SocialMedia from "@/components/SocialMedia.vue";
import Pages from "@/components/Pages.vue";
</script>

<template>
    <footer class="footer">
        <div class="footer__pages">
         <Pages />
        </div>
        <div class="footer__line" />
        <div class="footer__info">
          <Logo class="footer__info-logo" footer-logo />
          <span>Copyright ©2024 Все права защищены | STEPPE Art&Music</span>
          <div class="footer__info-social">
            <SocialMedia />
          </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
.footer {
  display: flex;
  gap: 40px;
  flex-direction: column;
  padding: 80px 0 50px 0;
  &__pages {
    display: flex;
    justify-content: center;
    gap: 50px;
  }
  &__line {
    width: 100%;
    height: 1px;
    background-color: $dark-400;
  }
  &__info {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    width: 100%;
    align-items: center;
    justify-content: space-between;
    span {
      display: flex;
      justify-content: center;
    }
    &-social {
      display: flex;
      align-items: center;
      gap: 30px;
      justify-content: flex-end;
    }
  }
}

</style>