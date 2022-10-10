<template>
  <h1>HellosWorld con prueba calculadora</h1>
  {{msg}}
  <br>
  Contador: {{counter}}
  <div>
    <button @click="appear()">Boton</button>
  
    <button @click="sumar()" style ="{backgroundColor: 'blue', color:'#fff'}" >+</button>
    <button @click="resta()">-</button>
    <button @click="reset()">Reset</button>
  </div>
</template>
<script>
export default {
  data() {
    return {
      msg: "Hola Mundo",
      counter: 0
    }
  },
  methods: {
    appear() {
      console.log("Hola Mundo")
    },
    sumar() {
            this.counter++;
        },
        resta() {
            this.counter--;
        },
        reset() {
            this.counter = 0
        }

  }
};

</script>
<style>

</style>