<template>
  <div>
    <NuxtRouteAnnouncer />
    <MovieBackground>
      <swiper-container>
        <swiper-slide></swiper-slide>
        <swiper-slide>
          <Glass title="コミュニティによって得られるもの">
            <p>あいうえおかきくけこさしすせそ</p>
            <p>あいうえおかきくけこさしすせそ</p>
            <p>あいうえおかきくけこさしすせそ</p>
            <p>あいうえおかきくけこさしすせそ</p>
          </Glass>
        </swiper-slide>
        <swiper-slide><Glass title="2. たいとる" /></swiper-slide>
      </swiper-container>
    </MovieBackground>
  </div>
</template>

<script setup>
import { register } from 'swiper/element/bundle'
import MovieBackground from './components/MovieBackground.vue'
register()
</script>
