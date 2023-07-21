<template>
  <section class="container-fluid">
    <article class="row mt-4">
      <div class="col" style="max-height: 50rem;">
        <figure class="row d-flex align-items-start justify-content-center">
          <section class="col-md-4 col-sm-4">
            <img src="@/assets/landing/recurso20.jpg" class="img-fluid" alt="hermosa ropa">
            <section class="row d-flex justify-content-between">
              <div class="col-2 d-flex align-items-start mt-5 mb-5 p-0">
                <TextY />
              </div>
              <div class="col-9 mt-3">
                <figure>
                  <img src="@/assets/landing/recurso23.jpg" class="img-fluid" alt="Lindas gafas">
                </figure>
                <figure>
                  <img src="@/assets/landing/recurso24.jpg" class="img-fluid" alt="Lindas gafas">
                </figure>
              </div>
            </section>
          </section>
          <section class="col-md-4 col-sm-4" style="height: 35rem;">
            <img src="@/assets/landing/recurso22.jpg" class="img-fluid" alt="Lindo conjunto con bolso">
            <div class="d-flex flex-column justify-content-center align-items-center m-5">
              <p class="fs-4 fw-normal text-left p-2 truncate-on-small" style="max-width: 25ch;">
                Crea tus total looks camel para
                verte sofisticada y atemporal.
                Eleva tu look con accesorios
                artesanales.
              </p>
              <Button text="Comprar ahora" class="ml-0" />
            </div>
          </section>
        </figure>

        <div class="container-fluid brown" style="height: 50rem; position: relative;top: -50rem; z-index: -1;">
          <div class="d-flex flex-column align-items-center j5ustify-content-center "></div>
        </div>

      </div>
    </article>
  </section>
</template>

<script setup>
import TextY from '@/components/TextY.vue'
import { Button } from '@/components/'
</script>

<style lang="scss" scoped>
@media (max-width: 20ch) {
  .truncate-on-small {
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
}

@media (min-width: 15ch) {
  .truncate-on-small {
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    margin-left: 3rem;

  }
}
</style>