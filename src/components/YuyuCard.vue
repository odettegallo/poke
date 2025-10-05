<script setup>
const props = defineProps({
    nombre: {
        type: String,
        required: true
    },
    descripcion: {
        type: String,
        required: true
    }
});
</script>


<template>
    <section class="yuyu-card">
        <h2>{{ nombre }}</h2>
        <p>{{ descripcion }}</p>
    </section>
</template>

<style scoped>
.yuyu-card {
    /* Fondo más oscuro, como un pergamino antiguo o una noche de batalla */
    background-color: #1a1a1a; 
    border: 2px solid #5a0000; /* Borde rojo oscuro/sangre */
    border-radius: 4px; /* Bordes menos redondeados para un aspecto más clásico */
    padding: 18px;
    margin: 12px;
    /* Sombra con un color que evoque energía (Reiki/Youki) */
    box-shadow: 0 0 15px rgba(255, 0, 0, 0.4), 0 0 5px rgba(255, 255, 255, 0.2); 
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}   

/* Efecto al pasar el ratón para simular una carga de poder */
.yuyu-card:hover {
    transform: translateY(-5px); 
    box-shadow: 0 5px 20px rgba(255, 0, 0, 0.6), 0 0 10px rgba(255, 255, 255, 0.4);
    cursor: default;
}

.yuyu-card h2 {
    margin-top: 0;
    color: #4CAF50; /* Título en un verde brillante que contrasta */
    text-shadow: 1px 1px 2px #000; /* Sombra para resaltar */
    border-bottom: 2px dashed #ff0000; /* Línea separadora roja */
    padding-bottom: 8px;
    margin-bottom: 12px;
    font-family: 'Arial Black', sans-serif; /* Fuente más fuerte */
    letter-spacing: 1px;
}
.yuyu-card p {
    color: #e0e0e0; /* Texto en un gris claro para mejor legibilidad */
    line-height: 1.6;
    font-family: 'Verdana', sans-serif; /* Fuente clara y legible */
    font-size: 16px;
}
</style>