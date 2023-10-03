<template>
    <div class="mt-9 p-10">
      <div class="relative overflow-x-auto border shadow-md sm:rounded-lg">
        <table class="w-full text-sm text-left text-blue-100 dark:text-blue-100">
          <thead class="text-xs text-white uppercase bg-blue-600 dark:text-white">
            <tr>
              <th scope="col" class="px-6 py-3">
                Número
              </th>
              <th scope="col" class="px-6 py-3">
                Tipo
              </th>
              <th scope="col" class="px-6 py-3">
                Precio
              </th>
              <th scope="col" class="px-6 py-3">
                Disponibilidad
              </th>
              <th scope="col" class="px-6 py-3">
                Acción
              </th>
            </tr>
          </thead>
          <tbody>
            <tr class="bg-blue-500 border-b border-blue-400">
              <td class="px-6 py-4 font-medium text-blue-50 whitespace-nowrap dark:text-blue-100">
                101
              </td>
              <td class="px-6 py-4">
                Individual
              </td>
              <td class="px-6 py-4">
                $100
              </td>
              <td class="px-6 py-4">
                Disponible
              </td>
              <td class="px-6 py-4">
            <a href="/detalle-habitaciones" class="font-medium text-white hover:underline">
              <i class="fas fa-eye"></i>               
              <font-awesome-icon icon="fa-solid fa-eye" />
            </a>
            <a href="/edit-habitacion" class="font-medium text-white hover:underline ml-2">
              <i class="fas fa-edit"></i> 
              <font-awesome-icon icon="fa-solid fa-pen-to-square" />
            </a>
            <a @click="showAlert" class="font-medium text-white hover:underline ml-2">
              <i class="fas fa-trash"></i> <!-- Icono de basura para "Eliminar" -->
              <font-awesome-icon icon="fa-solid fa-trash" />
            </a>
          </td>
            </tr>
            <tr class="bg-blue-500 border-b border-blue-400">
              <td class="px-6 py-4 font-medium text-blue-50 whitespace-nowrap dark:text-blue-100">
                102
              </td>
              <td class="px-6 py-4">
                Doble
              </td>
              <td class="px-6 py-4">
                $150
              </td>
              <td class="px-6 py-4">
                Disponible
              </td>
              <td class="px-6 py-4">
            <a href="/detalle-habitaciones" class="font-medium text-white hover:underline">
              <i class="fas fa-eye"></i>               
              <font-awesome-icon icon="fa-solid fa-eye" />
            </a>
            <a href="/edit-habitacion" class="font-medium text-white hover:underline ml-2">
              <i class="fas fa-edit"></i> 
              <font-awesome-icon icon="fa-solid fa-pen-to-square" />
            </a>
            <a @click="showAlert" class="font-medium text-white hover:underline ml-2">
              <i class="fas fa-trash"></i> <!-- Icono de basura para "Eliminar" -->
              <font-awesome-icon icon="fa-solid fa-trash" />
            </a>
          </td>
            </tr>
            <!-- Puedes agregar más filas con datos aquí -->
          </tbody>
        </table>
        <a href="/crear"><button  type="button"  class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-4 py-2 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800 m-4 p-4">Crear Habitacion</button></a>
      </div>
    </div>
  </template>
  
  <script>
  export default {
  name:'SweetAlert2',
  methods: {

    
    
    showAlert() {
    
    //this.$swal('Desea eliminar esta Habitacion?');

    this.$swal({title: 'Cuidado!!',
      text: "¿Desea eliminar esta Habitacion?",
      icon: 'warning',
      showCancelButton: true,
      confirmButtonColor: '#3085d6',
      cancelButtonColor: '#d33',
      confirmButtonText: 'Si',
      cancelButtonText: 'Cancelar'
    }).then((result) => {
          if(result.value) {
            this.$swal('Enhorabuena', 'Eliminado con exito', 'success')
          }
        });


    
  },
  }
}
</script>