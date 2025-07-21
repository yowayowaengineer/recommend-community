<template>
  <div class="h-screen w-screen flex justify-center items-center">
    <div class="glass">
      <h1>{{ title }}</h1>
      <div class="mt-8 flex flex-col gap-2">
        <slot />
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title?: string
}>()
</script>

<style lang="css" scoped>
.glass {
  width: 80%;
  height: 80vh;
  padding: 4rem 6rem;
  background-color: rgba(255, 255, 255, 0.1);
  border: 1px solid rgba(255, 255, 255, 0.4);
  border-right-color: rgba(255, 255, 255, 0.2);
  border-bottom-color: rgba(255, 255, 255, 0.2);
  border-radius: 10px;
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  line-height: normal;
}

.glass h1 {
  text-align: center;
  color: #fff;
  -webkit-text-stroke: 1px black;
  font-size: 50px;
  font-weight: bold;
  letter-spacing: 0.06em;
}

.glass div {
  color: #fff;
  text-shadow: 0 0 20px rgba(0, 0, 0, 0.7);
  font-size: 24px;
}
</style>
