<template>
  <section class="container-fluid" style="max-height: 1200px;">
    <article class="row d-flex align-items-center justify-content-center">
      <section class="row">
        <div class="col d-flex justify-content-center">
          <div class="row" style="max-width: 700px; position: static;">

            <Slider class="h-100" img1="slide02/recurso14.jpg" img2="slide02/recurso15.jpg"
              img3="slide02/recurso16.jpg" />

          </div>
        </div>
      </section>
      <figure class="card g-0 card-border-radius-none brown d-flex justify-content-end"
        style="max-width: 1000px; height: 65vh; position: relative;top: -12rem; max-height: 70vh; z-index: -1;">
        <div class="d-flex flex-column align-items-center j5ustify-content-center">
          <h2 class="display-2 text-center">
            Tonos de la tierra
          </h2>
          <p class="fs-4 text-center" style="max-width: 55ch;">
            Un estampado tropical con colores tierra es ideal para
            abrazar la nueva temporada.
          </p>
        </div>
      </figure>
    </article>
  </section>
  <!-- <main >
  </main> -->
</template>

<script setup>
import { Slider } from '@/components'
</script>

<style scoped></style>
