<template>
  <section class="container-fluid" style="max-height: 1070px;">
    <article class="row d-flex align-items-center justify-content-center">
      <figure class="card g-0 card-border-radius-none brown" style="max-width: 1000px; height: 60vh;">
        <div class="d-flex flex-column align-items-center justify-content-center">
          <h2 class="display-2 text-center">
            Alegría artesanal
          </h2>
          <p class="fs-4 text-center" style="max-width: 55ch;">
            Complementa tus looks llenos de color y alegría con
            <span class="fw-bolder">bolsos, accesorios y sandalias</span>
            que se inspiran en esta emocionante historia.
          </p>
        </div>
      </figure>
      <section class="row" style="position: relative;top:-11rem;">
        <div class="col d-flex align-items-center justify-content-center">
          <div class="row d-flex justify-content-center" style="max-width: 700px;">
            <div class="col-6">
              <picture class="d-flex align-items-center justify-content-center">
                <img src="@/assets/landing/recurso11.jpg" class="img-fluid m-3" alt="recurso 3">
              </picture>
              <picture class="d-flex align-items-center justify-content-center">
                <img src="@/assets/landing/recurso13.jpg" class="img-fluid m-3" alt="recurso 3">
              </picture>
            </div>
            <div class="col-6">
              <!-- <picture class="d-flex">
                <img src="@/assets/landing/recurso12.jpg" class="img-fluid ml-3 mt-n3" alt="recurso 3">
              </picture>

              <figure class="d-flex flex-column justify-content-center align-items-center">
                
              </figure> -->
              <picture class="d-flex align-items-center justify-content-start">
                <img src="@/assets/landing/recurso12.jpg" class="img-fluid m-3" alt="recurso 3">
              </picture>
              <div class="d-flex flex-column justify-content-center align-items-center m-3">
                <p class="fs-4 fw-normal text-left p-2">
                  Las texturas, fibras
                  naturales y efecto cuero
                  en tono crudo y tierra son
                  perfectos para exaltar las
                  prendas más coloridas
                </p>
                <Button text="Comprar ahora" class="p-2" />
              </div>

            </div>
          </div>
        </div>
      </section>
    </article>
  </section>
</template>

<script setup>
import Button from './Button.vue'
</script>

<style lang="scss" scoped></style>