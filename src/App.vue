<template>
  <main class="container-fluid m-0 slider-container">
    <SectionHeader />
    <Section1 />
    <Section2 />
  </main>
</template>
<script setup>
import { SectionHeader, Section1, Section2 } from './components'
</script>

<style scoped lang="scss">
.basic-snap-y {
  overflow-y: auto;
  scroll-snap-type: y mandatory;
  overscroll-behavior-y: contain;

  &>* {
    scroll-snap-align: center;
  }
}
</style>
