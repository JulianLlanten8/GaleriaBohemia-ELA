<template>
  <section class="container-fluid mt-5">
    <article class="row">
      <figure class="col d-flex align-items-center justify-content-center">
        <div class="card card-border-radius-none" style="max-width: 1000px;">
          <div class="row g-0 align-items-center">
            <div class="col-md-5 d-flex  flex-column align-items-center">
              <div class="card text-bg-dark mt-5">
                <img src="@/assets/landing/recurso3.jpg" style="height: 320px;" class="card-img" alt="...">
                <div class="card-img-overlay d-flex align-items-end justify-content-center ">
                  <p class="card-text">
                    <Button text="COMPRAR AHORA" />
                  </p>
                </div>
              </div>

              <div class="card text-bg-dark mt-5">
                <img src="@/assets/landing/recurso4.jpg" style="height: 320px;" class="card-img" alt="...">
                <div class="card-img-overlay d-flex align-items-end justify-content-center ">
                  <p class="card-text">
                    <Button text="COMPRAR AHORA" />
                  </p>
                </div>
              </div>
            </div>
            <div class="col-md-7">
              <Slider />
            </div>
          </div>
        </div>
      </figure>
    </article>
  </section>
</template>

<script setup>
import Button from './Button.vue'
import Slider from './Slider.vue'
</script>