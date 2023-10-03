<template>
  <div class="mt-9 p-10">
    <div class="container mx-auto">
      <h1 class="text-3xl font-semibold mt-5 mb-3">Crear Habitación</h1>
      <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
        <div>
          <div class="mb-4">
            <label class="block text-gray-700 text-sm font-bold mb-2" for="numero"
              >Número de Habitación:</label
            >
            <input
              type="text"
              id="numero"
              class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
              v-model="habitacion.numero"
              required
            />
          </div>
          <div class="mb-4">
            <label class="block text-gray-700 text-sm font-bold mb-2" for="tipo"
              >Tipo de Habitación:</label
            >
            <select
              id="tipo"
              class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
              v-model="habitacion.tipo"
              required
            >
              <!-- Opciones para el tipo de habitación -->
            </select>
          </div>
          <label class="block text-gray-700 text-sm font-bold mb-2" for="tipo">Acomodacion:</label>
          <select
            id="tipo"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            v-model="habitacion.tipo"
            required
          >
            <!-- Opciones para el tipo de acomodacion -->
          </select>
        </div>
        <div>
          <!-- Otros campos relacionados con la habitación -->
        </div>
      </div>
      <div class="mt-4">
        <a href="/"
          ><button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
            Guardar Habitación
          </button></a
        >
      </div>
    </div>
  </div>
</template>
  
  <script>
export default {
  data() {
    return {
      habitacion: {
        numero: '',
        tipo: '' // Puedes definir las opciones en data o cargarlas desde una API
        // Otros campos relacionados con la habitación
      }
    }
  },
  methods: {
    guardarHabitacion() {
      // Envía los datos de la habitación al backend para su creación
      // Luego, redirige a la lista de habitaciones
    }
  }
}
</script>
  