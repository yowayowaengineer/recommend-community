<template>
  <div>
    <NuxtRouteAnnouncer />
    <MovieBackground>
      <swiper-container>
        <swiper-slide></swiper-slide>
        <swiper-slide>
          <Glass title="あぁ、なんか面白そうなことやってる、を作りたい（切実）">
            <div class="flex flex-col justify-end items-center h-[50vh] gap-4">
              <p>イノベーション推進事業本部　デジタル推進部</p>
              <p>コンテスト実行委員会　顧問</p>
              <p>くらもとやすひろ</p>
              <p class="text-xl">@yowayowa_engr</p>
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
          <Glass title="前回のゲームコンテストとの違い">
            <div
              class="grid grid-cols-3 gap-4 text-center mt-12 items-center h-[40vh]"
            >
              <div>2021年</div>
              <div class="flex justify-center">
                <img src="/image/yajirushi.webp" alt="yajirushi" class="h-10" />
              </div>
              <div>2025年</div>

              <div>期間が1年</div>
              <div class="flex justify-center">
                <img src="/image/yajirushi.webp" alt="yajirushi" class="h-10" />
              </div>
              <div>期間が2年</div>

              <div>制作コンテスト</div>
              <div class="flex justify-center">
                <img src="/image/yajirushi.webp" alt="yajirushi" class="h-10" />
              </div>
              <div>ビジネスコンテスト</div>

              <div>短期集中で審査</div>
              <div class="flex justify-center">
                <img src="/image/yajirushi.webp" alt="yajirushi" class="h-10" />
              </div>
              <div>ゲームプラットフォームによるレビュー</div>
            </div>
          </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="どうしてそのような発想が生まれたのか？">
            <div
              class="flex flex-col justify-center items-center h-[50vh] gap-4"
            >
              <p>Godot Engineのコミュニティでのとある人のひとこと……</p>
              <br />
              <p>「個人ゲーム開発はプロダクトを自分で持っているようなもの」</p>
              <p>
                「自分のプロダクトを販売して、ユーザーの声を聞いて改善して（つまりは運営して）」
              </p>
              <p>「この経験は本業（同業）でもめっちゃ役に立つ」</p>
            </div>
          </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="どうしてそのような発想が生まれたのか？（その２）">
            <div
              class="flex flex-col justify-center items-center h-[50vh] gap-4"
            >
              <p>弊社社長の新年のあいさつ……</p>
              <br />
              <p>「倉敷から世界を目指す」</p>
              <p>「新しいことをする際にいきなり世界は難しい」</p>
              <p>「日本、お付き合いのある企業さまでも難しい」</p>
              <p>「社内で心理的安全性を確保して挑戦できる、それが委員会」</p>
            </div>
          </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="自分の視点と他者の視点">
            <div class="flex flex-col items-center h-[50vh] gap-8">
              <p>自分が思っている視点は普遍ではないということ。</p>
              <p>他者は違う視点でものごとを捉えているかもしれない。</p>
              <p>自分自身ですら状況が変わると視点が変わるかもしれない。</p>
              <img src="/image/shiten.webp" alt="shiten" class="mt-8 w-[50%]" />
              <p class="text-xs">
                画像：METAL GEAR SOLID 3 SNAKE EATER (MASTER COLLECTION版) -
                オンラインマニュアル「カメラ」（
                https://metalgear.konami.net/manual/mc1/mgs3/pc/ja/page13.html
                ）より引用。©2023 Konami Digital Entertainment
              </p>
            </div>
          </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="視野を広げることができるのが、そう……"> </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="コミュニティ参加のすゝめ">
            <div
              class="grid grid-cols-2 gap-4 text-center mt-12 items-center h-[40vh]"
            >
              <div class="flex justify-center">
                <img src="/image/xtalk.webp" alt="yajirushi" class="w-[25vw]" />
              </div>
              <div class="flex justify-center">
                <img src="/image/oso.webp" alt="yajirushi" class="w-[25vw]" />
              </div>
            </div>
          </Glass>
        </swiper-slide>
        <swiper-slide>
          <Glass title="蛇足">
            <div
              class="flex flex-col justify-center items-center h-[50vh] gap-4"
            >
              <p>なんか Nuxt4 が正式リリースされてた。</p>
              <p>なかなかよいぞ！</p>
            </div>
          </Glass>
        </swiper-slide>
        <swiper-slide></swiper-slide>
      </swiper-container>
    </MovieBackground>
  </div>
</template>

<script lang="ts" setup>
import { register } from 'swiper/element/bundle'
register()

useSeoMeta({
  // テスト環境用設定
  robots: () => {
    return { noindex: true }
  },
})
</script>
