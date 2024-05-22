<!-- <script setup>

import { ref } from 'vue';


let fechaInput = ref('')
let pesoInput = ref('')
let cinturaInput = ref('')
let caderaInput = ref('')

let pesoPerdido = ref(0)
let caderaPerdida = ref(0)
let cinturaPerdida = ref(0)


let listDatos = ref([{
fecha: '10 de junio de 2023',
peso: 80,
cintura: 78,
cadera: 86,
}])

function addDates() {
  if (fechaInput.value.trim() === '') {
    return {};
  } else {
    listDatos.value.push({
      fecha: fechaInput.value,
      peso: parseInt(pesoInput.value), 
      cintura: parseInt(cinturaInput.value), 
      cadera: parseInt(caderaInput.value) 
    });

    const ultimoDato = listDatos.value[listDatos.value.length - 1];

    if (listDatos.value.length > 1) {
      calculosPro(ultimoDato);
    }

 
  }
}





function calculosPro(ultimoDato) {
  const penultimoDato = listDatos.value[listDatos.value.length - 2];

  if (penultimoDato.peso >= ultimoDato.peso) {
    pesoPerdido.value = penultimoDato.peso - ultimoDato.peso;
  }

  if (penultimoDato.cintura >= ultimoDato.cintura) {
    cinturaPerdida.value = penultimoDato.cintura - ultimoDato.cintura;
  }

  if (penultimoDato.cadera >= ultimoDato.cadera) {
    caderaPerdida.value = penultimoDato.cadera - ultimoDato.cadera;
  }

  console.log("pesoPer " + pesoPerdido.value);
  console.log("Cadera " + caderaPerdida.value);
  console.log("CinturaP " + cinturaPerdida.value);
}




</script>

<template> -->














  <!-- <div class="bg-green-300 w-44 mb-3 ml-4">
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
  </div> -->

  <!-- <div v-for="(date,index) in listDatos" :key="index"
  class="bg-green-300 w-56 mb-3 ml-4">
    <ul> {{date.fecha }}</ul>
    <ul> Peso: {{ date.peso }}</ul>
    <ul>Cintura: {{ date.cintura }}</ul>
    <ul>Cadera: {{ date.cadera }}</ul>
  </div>




  <div>
    Peso perdido: {{ pesoPerdido }} | Reducción Cintura: {{ cinturaPerdida }} | Reducción cadera: {{ caderaPerdida }}
  </div>


  <div class="bg-green-300 w-56 h-60 ml-4 text-center">
    
    <input v-model="fechaInput" class="mt-2 mb-2 border-2  "type="text" placeholder="Fecha">
    <input v-model="pesoInput" class="mb-2 border-2"type="text" placeholder="Peso">
    <input v-model="cinturaInput" class="mb-2 border-2"type="text" placeholder="Talla Cintura">
    <input v-model="caderaInput" class="mb-2 border-2"type="text" placeholder="Talla Cadera">
    <button @click="addDates" class="border-2-black bg-white" >Añadir</button>
  </div>



  

</template> -->