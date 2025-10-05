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
    border: 1px solid #ccc;
    border-radius: 8px;
    padding: 16px;
    margin: 8px;
    box-shadow: 2px 2px 12px rgba(0, 0, 0, 0.1);
    background-color: #f9f9f9;
}   
.yuyu-card h2 {
    margin-top: 0;
    color: #333;
}
.yuyu-card p {
    color: #666;
    line-height: 1.4;
}
</style>