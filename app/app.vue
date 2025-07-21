<template>
  <div>
    <NuxtRouteAnnouncer />
    <MovieBackground>
      <swiper-container>
        <swiper-slide></swiper-slide>
        <swiper-slide>
          <Glass title="コミュニティによって得られるもの">
            <div
              class="flex flex-col justify-center items-center h-[50vh] gap-4"
            >
              <p>イノベーション推進事業本部　デジタル推進部</p>
              <p>コンテスト実行委員会　顧問</p>
              <p>くらもとやすひろ</p>
            </div>
          </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="今年のコンテストどう思う？">
            <ImageViewer
              src="/image/pic_promotion.webp"
              alt="PIC GAME AWARD 2025"
            />
          </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="前回のゲームコンテストとの違い"> </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="どうしてそのような発想が生まれたのか？"> </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="自分の視点と他者の視点"> </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="視野を広げることができるのが、そう……"> </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="コミュニティ参加のすゝめ"> </Glass>
        </swiper-slide>
        <swiper-slide></swiper-slide>
      </swiper-container>
    </MovieBackground>
  </div>
</template>

<script lang="ts" setup>
import { register } from 'swiper/element/bundle'
register()
</script>
