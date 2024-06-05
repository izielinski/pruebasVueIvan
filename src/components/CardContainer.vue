<template>
  <div class="CContainer">
    <CardContent />
    <CardContent />
    <CardContent />
    <CardContent />
  </div>
</template>

<script setup>
import CardContent from "./CardContent";
</script>

<style scoped>
.CContainer {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
}
</style>
