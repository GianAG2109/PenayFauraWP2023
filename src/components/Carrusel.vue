<template>
<div>
<v-carousel show-arrows="hover">
  <v-carousel-item
    src="../public/Imagenes/Carrusel/carrusel1.jpg"
    cover
  ></v-carousel-item>

  <v-carousel-item
    src="../public/Imagenes/Carrusel/carrusel2.jpg"
    cover
  ></v-carousel-item>

  <v-carousel-item
    src="../public/Imagenes/Carrusel/carrusel3.jpg"
    cover
  ></v-carousel-item>

  <v-carousel-item
    src="../public/Imagenes/Carrusel/carrusel4.jpg"
    cover
  ></v-carousel-item>

  <v-carousel-item
    src="../public/Imagenes/Carrusel/carrusel5.jpg"
    cover
  ></v-carousel-item>

  <v-carousel-item
    src="../public/Imagenes/Carrusel/carrusel6.jpg"
    cover
  ></v-carousel-item>
</v-carousel>
</div>
</template>


<script>
  export default {
    data () {
      return {
        colors: [
          'primary',
          'secondary',
          'yellow darken-2',
          'red',
          'orange',
        ],
        model: 0,
      }
    },
  }
</script>
<style scoped>
.carousel-container {
  display: flex;
  justify-content: center; /* Centra horizontalmente el carrusel */
  align-items: center; /* Centra verticalmente el carrusel si es necesario */
  height: 100vh; /* Ajusta la altura según sea necesario */
}
</style>