<script setup lang="ts">
import Author from './components/Author.vue';
import Test from './components/Test.vue';
import HelloWorld from './components/HelloWorld.vue'
import Card from "./components/card.vue";
import progressButton from './components/progressButton.vue';
import navBar from './components/navBar.vue';

</script>

<template>
  <navBar />
  <HelloWorld msg="Vite + Vue" />
  <Author />
  <Test />
  <card> Contenu de ma Card </card>
  <progressButton> Click </progressButton>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

</style>
