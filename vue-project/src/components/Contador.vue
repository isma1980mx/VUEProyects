<template>
<h1>Hola maistro!</h1>
<p>{{ contador }}</p>
<button @click="incrementar">Incrementa</button>
<button @click="decrementar">Decrementa</button>
</template>

<script setup>
import {ref} from 'vue';
const contador = ref(0);
const incrementar = () =>{
  contador.value++;
}
const decrementar = () =>{
  contador.value--;
}
</script>

<style scoped>
  h1{
    font-size: 75px;
  }
  p{
    color: red;
    font-size: 65px;
  }
</style>
