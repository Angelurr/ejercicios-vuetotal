<script setup>
import { ref } from 'vue';

let total = ref(0)
const valueMotorcycle = 2000
const valueCars = 3000

const isActive = ref(true);

const parkingMotorcycles = ref([
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
]);

const parkingCars = ref([
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
    { green: true },
]);

function cambiarEstiloMoto(index) {
    parkingMotorcycles.value[index].green = !parkingMotorcycles.value[index].green;

    if(!parkingMotorcycles.value[index].green){
        total.value += valueMotorcycle
    }
   
}

function cambiarEstiloCars(index){
    parkingCars.value[index].green = !parkingCars.value[index].green;

    if(!parkingCars.value[index].green){
        total.value += valueCars 
    }
}




</script>


<template>
    <div class="flex bg-green-400 justify-center text-6xl mb-10">
        Parking
    </div>

    <div class="flex bg-green-200 justify-center text-6xl mb-10">
        Total: {{ total }}
    </div>

    <section class="max-w-6xl mx-auto grid grid-cols-2">

        <div class=" grid grid-cols-3 gap-4">

            <div @click="cambiarEstiloMoto(index)" v-for="(parkingM, index) in parkingMotorcycles" :key="index"
                :class="{ 'bg-red-400': !parkingM.green, 'bg-green-400': parkingM.green }"
                class="cursor-pointer h-32 w-20">
                Moto
            </div>

        </div>

        <div class=" grid grid-cols-4 gap-4">

            <div @click="cambiarEstiloCars(index)" v-for="(parkingC, index) in parkingCars" :key="index"
                :class="{ 'bg-red-400': !parkingC.green, 'bg-green-400': parkingC.green }"
                class="cursor-pointer h-32 w-32">
                Cars
            </div>
            
        </div>

    </section>
</template>