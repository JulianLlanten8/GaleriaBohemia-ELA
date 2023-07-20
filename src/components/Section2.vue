<template>
  <section class="container-fluid mt-5">
    <article class="row">
      <figure class="col d-flex align-items-center justify-content-center">
        <div class="card card-border-radius-none" style="max-width: 1000px;">
          <div class="row g-0 align-items-center justify-content-between">
            <div class="col-md-5 d-flex  flex-column align-items-center">

              <MiniCard textButton="COMPRAR AHORA" url="landing/recurso3.jpg" />

              <MiniCard textButton="COMPRAR AHORA" url="landing/recurso4.jpg" />

            </div>
            <div class="col-md-7">
              <Slider img1="slide01/recurso5.jpg" img2="slide01/recurso6.jpg" img3="slide01/recurso7.jpg" />
            </div>
          </div>
        </div>
      </figure>
    </article>
  </section>
</template>

<script setup>
import { Button, Slider, MiniCard } from '@/components'
</script>