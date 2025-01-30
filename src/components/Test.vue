<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  data() {
    return {
      compteur: 0
    };
  },
});
</script>

<template>
    <h2>Incrementer le boutton</h2>
    <div id="app">
        <input type="button" @click="compteur++" value="Click ici" />
    </div>
    <input type="number" placeholder="0" v-model="compteur"/>
  </template>
  

  
  <style scoped>
  h2 {
    color: red;
  }
  </style>