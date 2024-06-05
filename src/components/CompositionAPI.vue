<template>
  <br />
  <br />
  <br />
  <h1>CompostionAPI</h1>
  <h2>{{ contador }}</h2>
  <button @click="sumarContador">boton1</button>
</template>

<script>
import { defineComponent, ref } from "vue";
export default defineComponent({
  name: "CompostionAPI.vue",
  setup() {
    let contador = ref(0);
    const sumarContador = () => {
      contador.value++;
    };
    return { contador, sumarContador };
  },
});
</script>
