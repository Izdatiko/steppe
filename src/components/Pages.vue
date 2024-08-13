<script setup lang="ts">

</script>

<template>
  <router-link :to="{name: 'home'}">Проект</router-link>
  <router-link :to="{name: 'about'}">О нас</router-link>
  <router-link :to="{name: 'contacts'}">Контакты</router-link>
</template>

<style scoped lang="scss">
  a {
    font-size: 16px;
    font-weight: 500;
    line-height: 18.83px;
    text-align: left;
  }
</style>