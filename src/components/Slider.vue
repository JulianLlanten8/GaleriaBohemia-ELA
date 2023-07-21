<template>
  <section ref="carrusel" id="carouselExampleIndicators" class="carousel slide">
    <div class="carousel-indicators ">
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
        <img :src="resolveImg(img1)" class="d-block object-fit-cover w-100 img-fluid" alt="recurso5">
      </div>
      <div class="carousel-item">
        <img :src="resolveImg(img2)" class="d-block object-fit-cover w-100 img-fluid" alt="recurso6">
      </div>
      <div class="carousel-item">
        <img :src="resolveImg(img3)" class="d-block object-fit-cover w-100 img-fluid" alt="recurso7">
      </div>
    </div>
  </section>
</template>

<script setup>
import { onMounted, ref } from 'vue'
import { Carousel } from 'bootstrap'

defineProps({
  img1: {
    type: String,
    required: true
  },
  img2: {
    type: String,
    required: true
  },
  img3: {
    type: String,
    required: true
  }
})


const carrusel = ref(null)

const resolveImg = (img) => {
  return `src/assets/landing/${img}`
}

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