<script setup>

import {ref} from 'vue';
let total = ref(0)

let productos=ref([
    {
        producto: 'arroz',
        cantidad: 6,
        valor: 2000,
        vencimiento: '12 de febrero 2024' 
    },
    {
        producto: 'chocolate',
        cantidad: 7,
        valor: 3000,
        vencimiento: '12 de marzo 2024' 
    },
    {
        producto: 'yogurt',
        cantidad: 8,
        valor: 4000,
        vencimiento: '12 de abril 2024' 
    },
    {
        producto: 'queso',
        cantidad: 9,
        valor: 5000,
        vencimiento: '12 de mayo 2024' 
    }
]);

function vencer(index){
    // if(vencimiento.value <= '12 de febrero 2024'){
    //    vencer(index);
    // }

}

function totalProdutos(index){
total.value+=index.cantidad;
console.log(total.value)

}





</script>

<template>
    <div>
        <ul v-for="(obj,index) in productos" :key="index">
        {{ obj.producto }}
        <span v-if="vencer(index)">(¡A punto de vencer!)</span>
        
        </ul>
    </div>
    <p>Total de productos: {{ total }}</p>
    <p>Valor total del inventario: {{  }}</p>

</template>