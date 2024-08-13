<script setup lang="ts">
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import TimeInfo from "@/components/TimeInfo.vue";

</script>

<template>
  <Header />
  <div class="main">
    <div class="container">
     <router-view></router-view>
      <TimeInfo />
     <Footer />
    </div>
  </div>

</template>

<style lang="scss">
.main {
  a, p {
    color: $white;
  }
}
</style>