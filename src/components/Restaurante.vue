<!-- <script setup>
import { ref } from 'vue';
let indice=ref(0)
let restaurante = ref([
    {
        dia: 'lunes',
        desayuno: ['arepa','empanada','papa'],
        almuerzo: ['mondongo','carne','pollo'],
        cena: ['caldo','pan','perro']
    },
    {
        dia: 'martes',
        desayuno: ['a','e','p'],
        almuerzo: ['m','c','p'],
        cena: ['c','p','p']   
    },
    {
        dia: 'miercoles',
        desayuno: ['ar','em','pa'],
        almuerzo: ['mo','ca','po'],
        cena: ['ca','pa','pe']
    },
    {
        dia: 'jueves',
        desayuno: ['arepa','empanada','papa'],
        almuerzo: ['mondongo','carne','pollo'],
        cena: ['caldo','pan','perro']
    },
    {
        dia: 'viernes',
        desayuno: ['arepa','empanada','papa'],
        almuerzo: ['mondongo','carne','pollo'],
        cena: ['caldo','pan','perro']
    },
    {
        dia: 'sabado',
        desayuno: ['arepa','empanada','papa'],
        almuerzo: ['mondongo','carne','pollo'],
        cena: ['caldo','pan','perro']
    }
])
function ver(index){
    indice.value=index;
}


</script>

<template>
    
    
    

</template> -->











<!-- <script setup>
  import { ref } from 'vue';

  let indice=ref(0)
  let pepe=ref(0)
  let restaurante= ref([
    {
      dia:'lunes',
      desayuno: ['Arepa de Huevo', 'Empanada', 'Patacon'],
      almuerzo: ['Mondongo', 'Bandeja Paisa', 'Changua'],
      cena: ['Hamburguesa', 'Salchipapa', 'Hot-Dog']
          },
  {
    dia:'martes',
  desayuno: ['Arepa con huevo', 'Pan con queso', 'Croissant'],
  almuerzo:['Meesi', 'Antonio', 'xd'],
  cena:['uwu', 'onixan', 'quehacesxd']
},
{
  dia:'miercoles',
  desayuno:['tamal', 'buÃ±uelos', 'natilla'],
  almuerzo:['Hamburguesa', 'Salchipapa', 'Hot-Dog'],
  cena: ['pechuga', 'carne', 'lomo']
},
{
  dia:'jueves',
  desayuno: ['yuca', 'chicharron', 'pasta'],
  almuerzo: ['lechona', 'salchichon', 'tamal'],
  cena:['papa', 'xd', 'uwu']
},
{
  dia:'viernes',
  desayuno:['suero', 'queso', 'mantequilla'],
  almuerzo: ['chorizo', 'fritanga', 'pescado'],
  cena: ['xd', 'xd', 'xd'],
},
{
dia:'sabado',
  desayuno: ['manzana', 'pera', 'mandarina'],
  almuerzo: ['morcilla', 'arroz', 'pasta'],
  cena: ['no hay cenas']
}])

 

    function ver(i){
      indice.value=i
    }
    function escoger(i){
      pepe.value=i
    }
</script>

<template>
 <h1 class="bg-gray-500 text-center font-medium uppercase text-4xl ">restaurante universitario </h1>
  <div class=" mt-6 flex justify-center w-[50%] mx-auto">
    <div class="w-[30%]">
      <div v-for="(obj,i) in restaurante" :key="i" class="" @click="ver(i)">
        <div v-if="indice==i" class="bg-sky-400 mt-2 py-1 px-2">{{ restaurante[i].dia }}</div>
        <div v-else class="bg-gray-500/30 mt-2 px-2 py-1">{{ restaurante[i].dia }}</div>
      </div>
    </div>
    <div class="w-[70%] bg-sky-400 mt-2">
      <div class="flex gap-5  ml-8">
        <p @click="escoger(0)" v-if="pepe==0" class="cursor-pointer p-1 bg-sky-700/80">Desayuno</p>
        <p @click="escoger(0)" v-else class="cursor-pointer p-1 ">Desayuno</p>
        <p @click="escoger(1)" v-if="pepe==1" class="cursor-pointer p-1 bg-sky-700/80">Almuerzo</p>
        <p @click="escoger(1)" v-else class="cursor-pointer p-1 ">Almuerzo</p>
        <p @click="escoger(2)" v-if="pepe==2" class="cursor-pointer p-1 bg-sky-700/80">Cena</p>
        <p @click="escoger(2)" v-else class="cursor-pointer p-1 ">Cena</p>
        
      </div>
      <ul v-for="(obj,i) in restaurante[indice].desayuno" :key="i" class="ml-4">
        <li v-if="pepe==0">
          {{ restaurante[indice].desayuno[i] }}
        </li>
        <li v-else-if="pepe==1">
          {{ restaurante[indice].almuerzo[i] }}
        </li>
        <li v-else>
          {{ restaurante[indice].cena[i] }}
        </li>
      </ul>
      
    </div>
  
  </div>
</template> -->