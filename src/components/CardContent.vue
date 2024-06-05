<template>
  <div class="Carta">
    <h3>Carta</h3>
    <p>Carta de prueba</p>
    <CardButton />
  </div>
</template>

<script setup>
import CardButton from "./CardButton.vue";
</script>

<style scoped>
/*scope sirve para que solo funcione el style para este componente*/

.Carta {
  width: 100%;
  border-radius: 10px;
  border: 1px solid;
  margin: 30px;
}
</style>
