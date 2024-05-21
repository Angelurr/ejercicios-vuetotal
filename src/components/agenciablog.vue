<!-- <script setup>

let objeto = {
   nota1:1,
   nota2:2,
   nota3:3,
   nota4:4,
   nota5:5,
   nota6:6

}





</script>
<style scoped>
.lista{
    display: flex;
    justify-content: space-between;

}


</style>

<template>
    <h1>bloque</h1>
<ul class="lista">
  
  <span  v-for="(obj, index) in objeto" :key="index">
  <li>{{ obj }}</li>
  </span>
</ul>

<h1>en lista</h1>
<ul class="bloque">
  
  <span  v-for="(obj, index) in objeto" :key="index">
  <li>{{ obj }}</li>
  </span>
</ul>

</template> -->