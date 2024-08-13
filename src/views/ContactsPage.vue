<script setup lang="ts">

</script>

<template>
<div>
  <div class="contacts">
    <div class="contacts__img">
      <img src="/img/about.png" alt="">
    </div>
  <div class="contacts__info">
    <div class="contacts__info-header">
      <h2>«Donec nulla erat, laoreet sit amet sodales a, lobortis vitae dui.»</h2>
    </div>
    <div class="contacts__info-text">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse ullamcorper sem quis massa aliquet,
        vel accumsan neque facilisis. Aliquam eget odio auctor, laoreet justo sed, interdum justo.
        Donec posuere vestibulum euismod. Sed finibus arcu vel rutrum dictum. In nec luctus metus,
        condimentum malesuada ex. Nam faucibus mauris nunc, sit amet condimentum ante accumsan a. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse ullamcorper sem quis massa aliquet,
        vel accumsan neque facilisis. Aliquam eget odio auctor, laoreet justo sed, interdum justo.
        Donec posuere vestibulum euismod. Sed finibus arcu vel rutrum dictum. In nec luctus metus,
        condimentum malesuada ex. Nam faucibus mauris nunc, sit amet condimentum ante accumsan a. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse ullamcorper sem quis massa aliquet,
        vel accumsan neque facilisis. Aliquam eget odio auctor, laoreet justo sed, interdum justo.
        Donec posuere vestibulum euismod. Sed finibus arcu vel rutrum dictum. In nec luctus metus,
        condimentum malesuada ex. Nam faucibus mauris nunc, sit amet condimentum ante accumsan a.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse ullamcorper sem quis massa aliquet,
        vel accumsan neque facilisis. Aliquam eget odio auctor, laoreet justo sed, interdum justo.
        Donec posuere vestibulum euismod. Sed finibus arcu vel rutrum dictum. In nec luctus metus,
        condimentum malesuada ex. Nam faucibus mauris nunc, sit amet condimentum ante accumsan a. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse ullamcorper sem quis massa aliquet,
        vel accumsan neque facilisis. Aliquam eget odio auctor, laoreet justo sed, interdum justo.
        Donec posuere vestibulum euismod. Sed finibus arcu vel rutrum dictum. In nec luctus metus,
        condimentum malesuada ex. Nam faucibus mauris nunc, sit amet condimentum ante accumsan a. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse ullamcorper sem quis massa aliquet,
        vel accumsan neque facilisis. Aliquam eget odio auctor, laoreet justo sed, interdum justo.
        Donec posuere vestibulum euismod. Sed finibus arcu vel rutrum dictum. In nec luctus metus,
        condimentum malesuada ex. Nam faucibus mauris nunc, sit amet condimentum ante accumsan a.
      </p>
    </div>
  </div>
  </div>
</div>
</template>

<style scoped lang="scss">
.contacts {
  display: flex;
  gap: 50px;
  padding-bottom: 80px;
  &__img {
      width: 850px;
  }
  &__info {
    color: $main-color;
    padding-top: 40px;
    &-header {
      font-size: 36px;
      font-weight: 700;
      line-height: 43.52px;
      text-align: left;
      padding-bottom: 30px;
    }
    &-text {
      display: flex;
      flex-direction: column;
      gap: 20px;
      p {
        color: $main-color;
      }
    }
  }
}
</style>