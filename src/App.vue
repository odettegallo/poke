<script setup>
import YuyuHakushoList from './components/YuyuHakushoList.vue';


const personajesYuYuHakusho = [
  {
    id: 1,
    nombre: "Yusuke Urameshi",
    descripcion: "Adolescente rebelde que muere salvando a un niño y es reclutado como Detective del Mundo Espiritual. Heredero de Raizen, posee gran poder espiritual y demoníaco. Su técnica principal es el Ray-gun."
  },
  {
    id: 2,
    nombre: "Kazuma Kuwabara",
    descripcion: "Compañero de escuela de Yusuke, inicialmente su rival. Humano con alto nivel de reiki, capaz de invocar una Espada Espiritual. Tiene un carácter noble y es muy leal a sus amigos."
  },
  {
    id: 3,
    nombre: "Kurama",
    descripcion: "Zorro demonio astuto que reencarna en un humano. Inteligente y estratégico, domina técnicas con plantas demoníacas. Su dualidad entre humano y demonio lo hace un personaje complejo."
  },
  {
    id: 4,
    nombre: "Hiei",
    descripcion: "Demonio de fuego con espada, rápido y letal. Hermano de Yukina, aunque lo oculta. Prefiere trabajar solo, pero demuestra lealtad a su equipo. Su técnica principal es el Dragón de la Llama Negra."
  },
  {
    id: 5,
    nombre: "Koenma",
    descripcion: "Príncipe del Mundo Espiritual, hijo del Rey Enma. Aunque parece un niño, tiene gran autoridad. Supervisa a Yusuke y otros detectives espirituales, usando su sello para purificar almas."
  },
  {
    id: 6,
    nombre: "Genkai",
    descripcion: "Maestra de artes espirituales y mentora de Yusuke. Sabia y estricta, transmite técnicas avanzadas como la Onda Espiritual. Su historia revela una juventud marcada por el combate y la pérdida."
  },
  {
    id: 7,
    nombre: "Yukina",
    descripcion: "Mujer de Hielo con poderes curativos. Hermana de Hiei, aunque no lo sabe. Su dulzura y compasión contrastan con el mundo violento que la rodea. Kuwabara está enamorado de ella."
  }
];


</script>

<template>
  <h1>Lista de Personajes de Yuyu Hakusho</h1>
  <YuyuHakushoList :personajes="personajesYuYuHakusho" />
</template>

<style>
/* Estilos globales para todo el cuerpo de la página */
body {
    background-color: #000000; /* Fondo negro para el contraste dramático */
    color: #fff; /* Texto blanco por defecto */
    font-family: 'Arial', sans-serif;
}

/* Estilo para el título principal */
h1 {
    text-align: center;
    color: #ff0000; /* Rojo vibrante como el "Rei-gun" de Yusuke */
    text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.3), 0 0 10px #31150b;
    margin-top: 20px;
    margin-bottom: 40px;
    font-size: 2.5em;
    border-bottom: 3px solid #4CAF50; /* Línea inferior verde */
    display: inline-block;
    padding: 0 20px 10px 20px;
    width: fit-content;
    margin-left: auto;
    margin-right: auto;
}

#app {
    max-width: 1200px; /* Limita el ancho del contenedor */
    margin: 0 auto;
    padding: 20px;
}

</style>
