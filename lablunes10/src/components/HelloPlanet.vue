<template>
    <h1>Hello Planet con prueba calculadora</h1>
    {{msg}}
    <br>
    Contador: {{counter}}
    <div>
        <button @click="appear()">Boton</button>
        <br>
        <button @click="sumar()">+</button>
        <button @click="resta()">-</button>
        <button @click="reset()">Reset</button>
        
    </div>
</template>
<script setup>
import { ref } from 'vue'
const counter = ref(0);

const appear= () => {
    console.log("Hola Mundo")
}
const msg = "Hola Mundo"

const sumar = () => {
    counter.value++;
}
const resta = () => {
    counter.value--
}
const reset = () => {
    counter.value = 0;
}

    
</script>
<style>

</style>