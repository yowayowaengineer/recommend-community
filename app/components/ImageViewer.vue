<template>
  <div class="image-container">
    <img :src="src" :style="imageStyle" @click="toggleZoom" />
  </div>
</template>

<script lang="ts" setup>
defineProps<{
  src: string
  alt?: string
}>()

const isZoomed = ref(false)

const toggleZoom = () => {
  isZoomed.value = !isZoomed.value
}

const imageStyle = computed(() => {
  return isZoomed.value
    ? {
        transform: 'scale(1.25)',
        position: 'absolute',
        left: '0px',
        top: '0px',
      }
    : {}
})
</script>

<style lang="css" scoped>
.image-container {
  width: auto;
  height: 50vh;
  overflow: hidden;
}

img {
  width: 100%;
  height: 100%;
  object-fit: contain;
  transition: transform 0.3s ease;
  cursor: pointer;
}
</style>
