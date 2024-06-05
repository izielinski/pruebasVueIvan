<template>
  <div>
    <h1>Option API</h1>
    <h2>{{ contador }}</h2>
    <br />
    <br />
    <br />
    <h2>{{ contador2 }}</h2>

    <button @click="agregarContador1">boton1</button>
    <button @click="agregarContador2">boton2</button>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "OptionsAPI",
  components: {
    // compo1, compo2, compo3
  },
  data() {
    let contador = 0;
    let contador2 = 2;

    return {
      contador,
      contador2,
    };
  },
  methods: {
    agregarContador1() {
      this.contador++;
    },
    agregarContador2() {
      this.contador2--;
    },
  },
});
</script>

<style>
/* Add your styles here */
</style>
