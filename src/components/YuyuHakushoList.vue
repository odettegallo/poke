<script setup>
const props = defineProps({
  personajes: {
    type: Array,
    required: true
  }
});

</script>

<template>
<section>
  <ul>
    <li v-for="personaje in personajes" :key="personaje.id">
      <h2>{{ personaje.nombre }}</h2>
      <p>{{ personaje.descripcion }}</p>
    </li>
  </ul>
</section>

</template>