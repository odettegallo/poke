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