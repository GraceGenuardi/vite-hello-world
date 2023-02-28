<template>
    <div class="bg-red">
      {{ description }}
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        description: 'La mia prima app con Vite!'
      }
    }
  }
  </script>
  
  <style>
  .bg-red {
    background-color: red;
    color: white;
  }
  </style>
  