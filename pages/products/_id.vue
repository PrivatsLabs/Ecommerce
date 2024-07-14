<template>
    <div>
      <h1>Product Detail</h1>
      <p>Product ID: {{ id }}</p>
      <!-- Add more details about the product here -->
    </div>
  </template>
  
  <script>
  export default {
    async asyncData({ params }) {
      return { id: params.id }
    }
  }
  </script>
  