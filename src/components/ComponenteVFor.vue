<template>
  <br />
  <br />
  <br />
  <h1>Estos son los jedis mas conocidos</h1>
  <h2 v-for="jedi in jedis" :key="jedi">{{ jedi }}</h2>
  <!--Se realiza un for para no escribir todos los items -->
  <br />
  <br />
  <br />
  <h2 v-for="(sith, index) in siths" :key="sith">
    {{ sith }} y su nro de jedi es: {{ index }}
  </h2>
  <!--Se realiza un for y el segundo campo nos ayuda con su index y asi poder trabajarlo -->

  <h2 v-for="(usuarioFuerza, index) in usuariosFuerza" :key="usuarioFuerza">
    {{ usuarioFuerza }} es un usuario de la fuerza con posicion {{ index }}
  </h2>

  <h2 v-for="(usuarioFuerza, index) in usuariosFuerza" :key="usuarioFuerza">
    {{ usuarioFuerza }} es un usuario de la fuerza con posicion {{ index }}
  </h2>
</template>

<script setup>
import { ref } from "vue";
let jedis = ref([
  "Maestro obi wan",
  "Anakin SkyWalker",
  "Yoda",
  "Luke Skywalker",
]);

let siths = ref([
  "Darth Sidius",
  "Darth Vader",
  "Darth Maul",
  "Darth Tenebreous",
]);

let usuariosFuerza = ref([...jedis.value, ...siths.value]);
// Los ... se puede
</script>

<style scoped></style>
