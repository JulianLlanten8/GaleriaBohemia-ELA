<template>
  <section ref="carrusel" id="carouselExampleIndicators" class="carousel slide">
    <div class="carousel-indicators">
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0"
        class="active btn rounded-circle" aria-current="true" aria-label="Slide 1">
      </button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"
        class="btn rounded-circle">
      </button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"
        class="btn rounded-circle">
      </button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="@/assets/landing/slide01/recurso5.jpg" class="d-block w-100" alt="recurso5">
      </div>
      <div class="carousel-item">
        <img src="@/assets/landing/slide01/recurso6.jpg" class="d-block w-100" alt="recurso6">
      </div>
      <div class="carousel-item">
        <img src="@/assets/landing/slide01/recurso7.jpg" class="d-block w-100" alt="recurso7">
      </div>
    </div>
  </section>
</template>

<script setup>
// hacer mover el carousel
import { onMounted, ref } from 'vue'
import { Carousel } from 'bootstrap'

const carrusel = ref(null)

onMounted(() => {
  if (carrusel.value) {
    setInterval(() => {
      const carousel = new Carousel(carrusel.value)
      carousel.next()
    }, 3000)
  }
  // si el carrusel esta activo, entonces pone la clase active de color rojo en el boton
  carrusel.value.addEventListener('slid.bs.carousel', (e) => {
    const buttons = carrusel.value.querySelectorAll('.carousel-indicators button')
    buttons.forEach((button, index) => {
      index === e.to ? button.classList.add('active') : button.classList.remove('active');
    })
  })

});

</script>

<style lang="scss" scoped>
.carousel-indicators [data-bs-target] {
  width: 20px !important;
  height: 20px !important;
}

.carousel-indicators .active {
  opacity: 1;
  background-color: #c96053 !important;
}
</style>