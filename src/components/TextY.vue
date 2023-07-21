<template>
  <section>
    <h1 class="display-1 m-0 fw-normal ">Look camel</h1>
  </section>
</template>

<script setup>

</script>

<style lang="scss" scoped>
h1 {
  /* Establece el texto verticalmente, de arriba hacia abajo */
  writing-mode: vertical-rl;
  /* Asegura que el texto se muestre en el orden inverso */
  text-orientation: mixed;
  /* giro de 180° al texto */
  transform: rotate(180deg);
  /* aumenta el espacio entre letras */
  letter-spacing: 0.1em;
}
</style>