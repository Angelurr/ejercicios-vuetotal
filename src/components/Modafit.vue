<script setup>
let listDatos = [{
fecha: '10 de junio de 2023',
peso: 80,
cintura: 78,
cadera: 86,
},
{
fecha: '12 de julio de 2023',
peso: 78,
cintura: 76,
cadera: 84, 
},
{
fecha: '9 de agosto de 2023',
peso: 76,
cintura: 74,
cadera: 82,   
  
}]

</script>

<template>
  <div class="bg-green-300 w-44 mb-3 ml-4">
    <ul>
        <li>10 de junio de 2023</li>
        <li>Peso: 80kg</li>
        <li>Cintura: 78cm</li>
        <li>Cadera: 86cm</li>
    </ul>
  </div>
  <div class="bg-green-300 w-44 mb-3 ml-4">
    <ul>
        <li>12 de julio de 2023</li>
        <li>Peso: 78kg</li>
        <li>Cintura: 76cm</li>
        <li>Cadera: 84cm</li>
    </ul>
  </div>
  <div class="bg-green-300 w-44 mb-7 ml-4">
    <ul>
        <li>9 de agosto de 2023</li>
        <li>Peso: 76kg</li>
        <li>Cintura: 74cm</li>
        <li>Cadera: 82cm</li>
    </ul>
  </div>

  <div class="bg-green-300 w-56 h-60 ml-4 text-center">
    
    <input class="mt-2 mb-2 border-2"type="text">
    <input class="mb-2 border-2"type="text">
    <input class="mb-2 border-2"type="text">
    <input class="mb-2 border-2"type="text">
    <a class="border-2-black bg-white" href="">Añadir</a>
    
    
  </div>
  

</template>