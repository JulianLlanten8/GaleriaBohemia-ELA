<template>
  <picture class="card mt-5 card-border-radius-none">
    <img :src="resolveUrl(url)" style="height: 365px;" class="card-img card-border-radius-none mr-5" alt="...">
    <div class="card-img-overlay d-flex align-items-end justify-content-center ">
      <p class="card-text">
        <Button :text="textButton" />
      </p>
    </div>
  </picture>
</template>

<script setup>
import { onMounted } from 'vue'
import { Button } from '@/components'
defineProps({
  textButton: {
    type: String,
    required: true
  },
  url: {
    type: String,
    required: true
  }
})

const resolveUrl = (url) => {
  const u = new URL(`../assets/${url}`, import.meta.url).href
  return u;
}



</script>

<style lang="scss" scoped></style>