<template>
  <div>
    <NuxtRouteAnnouncer />
    <swiper-container>
      <swiper-slide><Glass /></swiper-slide>
      <swiper-slide>Slide 2</swiper-slide>
      <swiper-slide>Slide 3</swiper-slide>
    </swiper-container>
  </div>
</template>

<script setup>
import { register } from 'swiper/element/bundle'
register()
</script>

<style lang="css">
body {
  background: linear-gradient(65deg, #231557, #44107a, #ff1361, #fff800);
  background-size: 1000% 1000%;
  animation: GradientBackground 20s ease infinite;
}

@keyframes GradientBackground {
  0% {
    background-position: 0% 50%;
  }

  50% {
    background-position: 100% 50%;
  }

  100% {
    background-position: 0% 50%;
  }
}
</style>
