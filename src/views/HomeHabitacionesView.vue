<template>
  <div>
    <NavComp />
    
    <!-- Contenido de la página de inicio para las habitaciones -->
    <section>
      <h1>Bienvenido a nuestras habitaciones</h1>
      <!-- Puedes agregar contenido, como una lista de habitaciones destacadas, imágenes, etc. -->
      
      <!-- Agrega el componente ListarHabitacionesComp aquí -->
      <ListarHabitacionesComp />
    </section>
    
    <FooterComp />
  </div>
</template>

<script setup>
import NavComp from '../components/global/NavComp.vue';
import FooterComp from '../components/global/FootComp.vue';
import ListarHabitacionesComp from '../components/ListarHabitacionesComp.vue'; // Importa el componente ListarHabitacionesComp
</script>
