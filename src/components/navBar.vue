<template>
    <nav class="navbar">
      <ul class="navbar-list">
        <li v-for="(item, index) in items" :key="index" class="navbar-item">
          <a href="#" @click="handleClick(item)" class="navbar-link">
            {{ item }}
          </a>
        </li>
      </ul>
    </nav>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue';
  
  // Liste des éléments de la navbar
  const items = ref(['Home', 'About', 'Services', 'Contact']);
  
  // Fonction de gestion du clic
  const handleClick = (item: string) => {
    console.log(`${item} clicked!`);
  };
  </script>
  
  <style scoped>
  /* Style de la navbar */
  .navbar {
    background-color: #333;
    padding: 10px 20px;
  }
  
  .navbar-list {
    display: flex;
    list-style: none;
    padding: 0;
    margin: 0;
  }
  
  .navbar-item {
    margin-right: 20px;
  }
  
  .navbar-link {
    color: white;
    text-decoration: none;
    font-size: 18px;
    padding: 8px 16px;
    border-radius: 5px;
    transition: all 0.3s ease;
  }
  
  .navbar-link:hover {
    background-color: #555; /* Couleur de fond au survol */
    transform: scale(1.1); /* Effet de zoom au survol */
  }
  
  .navbar-link:active {
    background-color: #444; /* Changer la couleur au clic */
    transform: scale(1); /* Rétablir la taille au clic */
  }
  </style>
  