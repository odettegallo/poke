<script setup>
import YuyuCard from './YuyuCard.vue';

const props = defineProps({
  personajes: {
    type: Array,
    required: true
  }
});

</script>

<template>
<section class ="yuyu-hakusho-list">
<YuyuCard v-for="personaje in personajes" 
    :key="personaje.id"
    :nombre="personaje.nombre"
    :descripcion="personaje.descripcion" />
</section>

</template>

<style scoped>
.yuyu-hakusho-list {
    display: grid;
    /* Cuadrícula adaptable: 3 columnas en pantallas grandes, 2 en medianas, 1 en pequeñas */
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); 
    gap: 20px; /* Espacio entre las tarjetas */
    padding: 20px 0;
}
</style>