<script setup lang="ts">
import { ref, computed, onMounted, onUnmounted } from 'vue';

const totalSeconds = ref(123456789);

const countdown = computed(() => {
  const days = Math.floor(totalSeconds.value / (24 * 3600));
  const hours = Math.floor((totalSeconds.value % (24 * 3600)) / 3600);
  const minutes = Math.floor((totalSeconds.value % 3600) / 60);
  const seconds = Math.floor(totalSeconds.value % 60);

  return {
    days,
    hours,
    minutes,
    seconds
  };
});

const updateCountdown = () => {
  if (totalSeconds.value > 0) {
    totalSeconds.value--;
  } else {
    clearInterval(intervalId);
  }
};

let intervalId: number;

onMounted(() => {
  intervalId = setInterval(updateCountdown, 1000);
});

onUnmounted(() => {
  clearInterval(intervalId);
});
</script>

<template>
  <section class="time">
    <p>22, 23, 24 НОЯБРЯ 2024 ГОДА</p>
    <div class="time__info">
      <img src="/img/fest.png" alt="">
      <div class="time__timer">
        <div class="time__timer-countdown">
          <h4>{{countdown.days}}<span>Д.</span></h4>
          <h4>•</h4>
          <h4>{{countdown.hours}}<span>Ч.</span></h4>
          <h4>•</h4>
          <h4>{{countdown.minutes}}<span>МИН.</span></h4>
          <h4>•</h4>
          <h4>{{countdown.seconds}}<span>СЕК.</span></h4>
        </div>
      </div>

    </div>
  </section>
</template>

<style scoped lang="scss">
.time {
  display: flex;
  flex-direction: column;
  gap: 20px;

  p {
    font-size: 36px;
    font-weight: 500;
    letter-spacing: 1.25em;
    text-align: left;
    width: 100%;
    max-width: 100%;
    box-sizing: border-box;
    white-space: normal;
    overflow-wrap: break-word;
    word-break: break-all;
  }

  &__info {
    width: 100%;
    text-align: center;
    font-weight: bold;
    line-height: 1;

    img {
      max-width: 100%;
      position: relative;
      top: 5px;
    }

    h2 {
      color: $main-color;
    }
  }
  &__timer {
    display: flex;
    flex-direction: column;
    background-color: $main-color;
    container-type: inline-size;
      padding-bottom: 120px;
    &-countdown {
      display: flex;
      align-items: center;
      justify-content: space-between;
      h4 {
        margin-block: 0px;
        font-size: 12cqw;
        color: $dark;
        display: flex;
        flex-direction: column;
        span {
          font-size: 20px;
          font-weight: 500;
          line-height: 23.54px;
          text-align: right;
          color: $dark;
        }
      }

      span {
        display: inline-block;
      }
    }

    &-labels {
      display: flex;
      justify-content: space-around;
      font-size: 2vw;
      margin-top: 10px;

      span {
        margin: 0 5px;
      }
    }
  }
}
</style>
