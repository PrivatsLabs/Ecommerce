<!-- pages/products/_id.vue -->

<template>
  <div v-if="product">
    <h1>{{ product.nom }}</h1>
    <p>{{ product.info }}</p>
    <p>Prix: {{ product.prix }}</p>
    <img :src="product.url" alt="Image du produit">
    <!-- Autres détails du produit -->
  </div>
  <div v-else>
    <p>Chargement en cours...</p>
  </div>
</template>

<script>
// Importer les données depuis utils/data.js
import { items } from '~/utils/data.js';

export default {
  async asyncData({ params }) {
    try {
      const productId = params.id; // L'ID est une chaîne dans vos données
      const product = items.find(prod => prod.id === productId);
      return { product };
    } catch (error) {
      console.error('Erreur lors de la récupération des détails du produit', error);
      return { product: null };
    }
  }
};
</script>

<style>
/* Styles spécifiques au composant */
</style>
