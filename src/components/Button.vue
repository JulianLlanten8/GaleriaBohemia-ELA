<template>
  <button type="button" class='btn btn-ela text-white btn-lg px-5 rounded-pill'>
    {{ text.toUpperCase() }}
  </button>
</template>

<script setup>
defineProps({
  text: {
    type: String,
    required: true
  }
})

</script>

<style lang="scss" scoped></style>