<template>
  <div class="card">
    <div class="card-body">
      <!-- Le bouton avec des effets -->
      <button class="btn-effect" @click="handleClick">
        <slot>Click Me</slot>
      </button>
    </div>
  </div>
</template>

<script setup lang="ts">
const handleClick = () => {
  console.log("Button clicked!");
};
</script>

<style scoped>
/* Style du bouton avec des effets */
.btn-effect {
  background-color: #d41212; /* Couleur de fond */
  color: white; /* Couleur du texte */
  border: none;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  cursor: pointer;
  border-radius: 8px;
  transition: all 0.3s ease;
}

.btn-effect:hover {
  background-color: #ec9819; /* Changer la couleur au survol */
  transform: scale(1.1); /* Agrandir légèrement au survol */
}

.btn-effect:active {
  background-color: #cbeb1b; /* Couleur de fond au clic */
  transform: scale(1); /* Réduire l'agrandissement */
}
</style>
